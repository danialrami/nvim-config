# Neovim Configuration

Neovim configuration focused on development with LSP support, fuzzy finding, and a clean interface.

## Plugin List

### Core Plugins
- **lazy.nvim** - Plugin manager
- **catppuccin** - Color scheme
- **lualine.nvim** - Status line
- **neo-tree** - File explorer
- **telescope.nvim** - Fuzzy finder
- **nvim-treesitter** - Syntax highlighting
- **mason.nvim** - LSP package manager
- **dressing.nvim** - Enhanced UI for inputs and selects
- **ollama.nvim** - AI assistance integration

### LSP & Completion
- **nvim-lspconfig** - LSP configuration
- **mason-lspconfig** - Bridge between mason and lspconfig
- **nvim-cmp** - Completion engine
- **LuaSnip** - Snippet engine

## Keybindings

### General
- `Space` - Leader key
- `\` - Local leader key

### Neo-tree
- `Ctrl + n` - Toggle file explorer

### Telescope
- `Ctrl + p` - Find files
- `<leader>fg` - Live grep (find in files)
- `<leader>fb` - Find buffers

### Ollama
- `<leader>oo` - Open Ollama prompt
- `<leader>oG` - Generate code with Ollama

### LSP
- `K` - Hover documentation
- `gd` - Go to definition
- `gr` - Find references
- `<leader>ca` - Code actions
- `<leader>rn` - Rename symbol
- `[d` - Previous diagnostic
- `]d` - Next diagnostic

### Completion
- `Ctrl + Space` - Trigger completion
- `Ctrl + e` - Close completion window
- `Tab` - Next completion item
- `Shift + Tab` - Previous completion item
- `Enter` - Confirm completion
- `Ctrl + b` - Scroll docs up
- `Ctrl + f` - Scroll docs down

## Language Servers

Currently configured for:
- Lua
- Python
- Rust
- CSS
- HTML
- JSON
- Tailwind CSS
- C/C++

## Installation

1. Clone this repository to your Neovim config directory:
```
git clone https://github.com/danialrami/nvim-config.git ~/.config/nvim
```

2. Start Neovim:
```
nvim
```

Lazy.nvim will automatically install all plugins on first launch.

## Requirements

- Neovim >= 0.9.0
- Git
- A Nerd Font (for icons)
- ripgrep (for telescope live grep)
- curl (for ollama.nvim)
- Ollama server running locally
```