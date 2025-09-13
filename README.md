# Tmux

Customized terminal multiplexer setup with vim-like keybindings, session management, and theming options.

## Plugins

- None

## Integrations

- **tmux.nvim**: Neovim plugin for tmux integration
- **Sessionizer**: Custom script for project-based session management
- **Neovim**: Vim-aware pane navigation
- **Zsh**: Shell integration for session management

## Configuration

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

## System Dependencies

### Required

- **tmux** - Terminal multiplexer
- **zsh** - Shell for sessionizer script execution

### Optional

- **neovim/vim** - For vim-aware pane navigation
- **fzf** - For fuzzy project selection in sessionizer

## Installation

1. Ensure all system dependencies are installed
2. Clone or copy this configuration to `~/.config/tmux/`
3. Source the main config: `tmux source ~/.config/tmux/tmux.conf`
