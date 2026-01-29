# Rahul's MyBash Configuration

> 🏜️ **Fork of [ChrisTitusTech/mybash](https://github.com/ChrisTitusTech/mybash)** with Rajasthani-inspired dark pastel theme

![Rajasthani Theme Preview](https://img.shields.io/badge/Theme-Rajasthani%20Desert-9A7B5B?style=for-the-badge)

## ✨ What's Different?

This fork includes a custom **Rajasthani Desert** color theme designed for dark terminals:

| Element | Color | Hex |
|---------|-------|-----|
| Username/Python | Dark Gray | `#3B4252` |
| Directory | Medium Gray | `#434C5E` |
| Git Branch/Status | Dusty Bronze | `#9A7B5B` |
| Languages | Copper | `#B87333` |
| Docker Context | Antique Gold | `#C9A66B` |
| Time | Deep Mauve | `#6B4E4E` |

## 📦 Installation

### Quick Install (via Linutil)

If you're using [my Linutil fork](https://github.com/rahuljangirworks/linutil):

1. Run Linutil
2. Navigate to **"Rahul's Scripts"** tab
3. Select **"Rahul's MyBash Setup"**

### Manual Install

```bash
git clone https://github.com/rahuljangirworks/mybash.git ~/.local/share/mybash
cd ~/.local/share/mybash

# Backup existing config
mv ~/.bashrc ~/.bashrc.bak

# Link configs
ln -sf ~/.local/share/mybash/.bashrc ~/.bashrc
ln -sf ~/.local/share/mybash/starship.toml ~/.config/starship.toml
cp ~/.local/share/mybash/config.jsonc ~/.config/fastfetch/config.jsonc

# Reload shell
exec bash
```

## 📁 Files

| File | Purpose |
|------|---------|
| `.bashrc` | Main bash configuration |
| `.bashrc.local` | Personal customizations (safe from upstream conflicts) |
| `starship.toml` | Starship prompt with Rajasthani colors |
| `config.jsonc` | Fastfetch config with matching theme |

## 🔄 Syncing with Upstream

```bash
cd ~/.local/share/mybash
git fetch upstream
git rebase upstream/main
git push origin main --force-with-lease
```

## 🎨 Customization

Add personal aliases and functions to `.bashrc.local` - this file is safe from merge conflicts:

```bash
# Example ~/.bashrc.local
alias myalias='my-command'
export MY_VAR="value"
```

## 🙏 Credits

- Original: [ChrisTitusTech/mybash](https://github.com/ChrisTitusTech/mybash)
- Prompt: [Starship](https://starship.rs/)
- System Info: [Fastfetch](https://github.com/fastfetch-cli/fastfetch)