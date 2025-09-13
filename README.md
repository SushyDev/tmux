# Tmux

This tmux configuration provides a customized terminal multiplexer setup with vim-like keybindings, session management, and theming options.

## System Dependencies

- **tmux** - Terminal multiplexer (core dependency)
- **zsh** - Shell used for sessionizer script execution
- **neovim/vim** - Optional, For vim-aware pane navigation and integration features inside neovim itself

## Notable Configurations

### Keybindings
- **Prefix**: `Ctrl+Space` (instead of default `Ctrl+b`)
- **Vim mode**: Enabled for copy mode with vim-like navigation
- **Smart pane navigation**: Automatically detects vim and sends keys appropriately
- **Session picker**: `prefix + w` shows session tree instead of window list
- **Even layout**: `prefix + =` for horizontal even spacing
- **Sessionizer**: `prefix + space` runs custom sessionizer script

### Settings
- **Base index**: Windows and panes start at 1
- **Renumber windows**: Automatically renumbers windows when one is closed
- **Focus events**: Enabled for better integration with `tmux.nvim`
- **Escape time**: Set to 0 for instant key response
- **Detach on destroy**: Disabled to prevent terminal exit when killing sessions

### Themes
Two theme options available:
- **Monochromatic** (default): Clean grayscale theme
- **Vapor**: Colorful theme with magenta accents

To switch themes, edit `custom/theme.conf` to source the desired theme file.

## Installation

1. Ensure all system dependencies are installed
2. Clone or copy this configuration to `~/.config/tmux/`
3. Source the main config: `tmux source ~/.config/tmux/tmux.conf`

## Integration

This configuration includes integration features for:
- **tmux.nvim**: Neovim plugin for tmux integration
- **Sessionizer**: Custom script for project-based session management (requires `dev` command in PATH)
