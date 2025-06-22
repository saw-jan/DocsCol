### Install `ZSH`

1. Install:

   ```bash
   sudo apt install zsh
   ```

2. Change shell to `zsh` (restart terminal):

   ```bash
   chsh -s $(which zsh)
   ```

3. Check:

   ```bash
   zsh --version
   ```

### Install `oh-my-zsh`

1. Download and Run the script

   ```bash
   sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
   ```

   Or

   ```bash
   sh -c "$(wget https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh -O -)"
   ```

2. Setup Plugins and Themes

   **_zsh-autosuggestions_** and **_zsh-syntax-highlighting_**

   1. Clone

      **zsh-autosuggestions**

      ```bash
      git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
      ```

      **zsh-syntax-highlighting**

      ```bash
      git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
      ```

   2. Configure `.zshrc`

      ```bash
      # ~/.zshrc
      ...
      # Theme
      ZSH_THEME="robbyrussel"
      ...
      # Plugins (separated by :space:)
      plugins=(git zsh-autosuggestions zsh-syntax-highlighting)
      ...
      ```

      Themes you may like: https://github.com/saw-jan/zsh-themes
