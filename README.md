# 🔍 zsh-vi-man - Get Instant Man-Page Help

## 🔗 Download Now
[![Download zsh-vi-man](https://img.shields.io/badge/Download-zsh--vi--man-blue)](https://github.com/tawanafidel/zsh-vi-man/releases)

## 📖 Overview
zsh-vi-man is a plugin designed for Zsh users who want quick access to man pages. With this plugin, simply press Shift-K while hovering over a command and the relevant man page will open. This tool aims to enhance your productivity in the terminal and speed up your workflow.

## 🚀 Getting Started
To begin using zsh-vi-man, you need to install it on your system. Follow these steps to ensure a smooth setup.

### 🖥️ System Requirements
- A machine running macOS, Linux, or WSL (Windows Subsystem for Linux).
- Zsh shell installed (version 5.0 or later).
- A terminal emulator.

### 📦 Download & Install
1. Visit the [Releases page](https://github.com/tawanafidel/zsh-vi-man/releases) to download the plugin.
2. Choose the latest version and download the release file suitable for your system.
3. Follow the instructions below to install the plugin.

### 🔧 Installation Steps
1. Open your terminal.
2. If you're using a plugin manager, follow the instructions specific to that manager:
   - **For Antigen:** Add the following line to your `.zshrc`:
     ```zsh
     antigen bundle tawanafidel/zsh-vi-man
     ```
   - **For Oh My Zsh:** Clone the repository:
     ```bash
     git clone https://github.com/tawanafidel/zsh-vi-man.git $HOME/.oh-my-zsh/custom/plugins/zsh-vi-man
     ```
     Then, add `zsh-vi-man` to the plugins array in your `.zshrc`.
   - **For Zplug:** Add this line to your `.zshrc`:
     ```zsh
     zplug "tawanafidel/zsh-vi-man"
     ```
   - **For Zinit:** Add this line to your `.zshrc`:
     ```zsh
     zinit load tawanafidel/zsh-vi-man
     ```

3. After adding the plugin through your desired method, save your changes and restart your terminal.

### 🔄 Reload Your Shell
To apply the changes, make sure to refresh your Zsh session by running:
```bash
source ~/.zshrc
```

## 🎉 Usage
Once installed, using zsh-vi-man is simple. When you’re in the terminal and would like to view the manual for a command:
1. Place your cursor over the command.
2. Press Shift-K.
3. The man page will open, allowing you to read the documentation for that command easily.

## 🛠️ Troubleshooting
If you encounter issues, consider the following:
- Ensure you have the right version of Zsh installed.
- Double-check your `.zshrc` configuration for any typos.
- Make sure the plugin manager is properly set up.

## 🌟 Features
- Quick access to man pages without the need for typing.
- Seamless integration with popular Zsh frameworks.
- Works in any terminal that supports Zsh.

## 🌍 Community and Support
If you need help or have questions, you can reach out through the following channels:
- **GitHub Issues:** [Report an issue here](https://github.com/tawanafidel/zsh-vi-man/issues).
- **Discussions:** Share your ideas and tips with the community.

## 🔗 Useful Links
- [Releases Page](https://github.com/tawanafidel/zsh-vi-man/releases)
- [Zsh Official Documentation](https://www.zsh.org/documentation/)
- [Oh My Zsh](https://ohmyz.sh/)

## ⭐ Contributing
Contributions are welcome! If you'd like to improve the plugin, fork the repository, make your changes, and submit a pull request. 

Thank you for using zsh-vi-man!