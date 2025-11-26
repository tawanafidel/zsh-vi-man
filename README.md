# zsh-vi-man

A zsh plugin that provides smart man page lookup in vi mode. Press `K` on any command or option to instantly open its man page—just like in vim!

## Features

- **Smart man page detection** — Automatically finds the right man page for subcommands (e.g., `git commit` → `git-commit`)
- **Option jumping** — When your cursor is on an option like `-r` or `--recursive`, the man page opens directly at that option
- **Combined options support** — Works with combined short options like `-rf`
- **Long options with values** — Handles `--color=always` by searching for `--color`

## Installation

### [zinit](https://github.com/zdharma-continuum/zinit)

```zsh
zinit light TunaCuma/zsh-vi-man
```

### [antidote](https://github.com/mattmc3/antidote)

Add to your `.zsh_plugins.txt`:

```
TunaCuma/zsh-vi-man
```

### [oh-my-zsh](https://github.com/ohmyzsh/ohmyzsh)

Clone into your custom plugins directory:

```bash
git clone https://github.com/TunaCuma/zsh-vi-man ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-vi-man
```

Then add to your `.zshrc`:

```zsh
plugins=(... zsh-vi-man)
```

### Manual

```bash
git clone https://github.com/TunaCuma/zsh-vi-man ~/.zsh-vi-man
echo 'source ~/.zsh-vi-man/zsh-vi-man.plugin.zsh' >> ~/.zshrc
```

## Usage

1. Type a command (e.g., `ls -la` or `git commit --amend`)
2. Press `Escape` to enter vi normal mode
3. Move your cursor to any word
4. Press `K` to open the man page

### Examples

| Command Line      | Cursor On     | Result                                     |
|-------------------|---------------|--------------------------------------------|
| `ls -la`          | `ls`          | Opens `man ls`                             |
| `ls -la`          | `-la`         | Opens `man ls` and jumps to `-l` or `-a`   |
| `git commit`      | `commit`      | Opens `man git-commit`                     |
| `grep --color=auto` | `--color=auto` | Opens `man grep` and jumps to `--color` |

## Configuration

Set these variables **before** sourcing the plugin:

```zsh
# Change the trigger key (default: K)
ZVM_MAN_KEY='?'

# Use a different pager (default: less)
ZVM_MAN_PAGER='bat'
```

## Integration with zsh-vi-mode

This plugin works seamlessly with [zsh-vi-mode](https://github.com/jeffreytse/zsh-vi-mode). It automatically detects if zsh-vi-mode is loaded and hooks into its lazy keybindings system.

For best results, source this plugin **after** zsh-vi-mode:

```zsh
source /path/to/zsh-vi-mode.zsh
source /path/to/zsh-vi-man.zsh
```

## License

MIT License - see [LICENSE](LICENSE) for details.

