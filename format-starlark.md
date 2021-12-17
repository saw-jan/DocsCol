## Format starlark file

### Install Buildifier

1. Install `go` from [here](https://go.dev/doc/install)
2. Install `buildifier`

   ```bash
   go install github.com/bazelbuild/buildtools/buildifier@latest
   ```

   [How to use?](https://chromium.googlesource.com/external/github.com/bazelbuild/buildtools/+/HEAD/buildifier/README.md)

**Note:** If you see error: `command not found: buildifier` then copy buildifier executable from `~/go/bin/buildifier` to `/usr/local/bin`

### Use with VSCode

1. Open vscode `settings.json`
2. Add the following configs:

   ```json
   {
        ...

        "[starlark]": {
            "editor.defaultFormatter": "BazelBuild.vscode-bazel"
        },
        "bazel.buildifierExecutable": "/usr/local/bin/buildifier",

        ...
   }
   ```
