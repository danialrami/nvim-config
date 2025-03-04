# Neovim Configuration

Neovim configuration focused on development with fuzzy finding, LSP integration, SuperCollider audio programming, and AI-assisted coding.

## Plugin List

### Core Plugins
- **lazy.nvim** - Plugin manager
- **catppuccin** - Color scheme  
- **lualine.nvim** - Status line
- **neo-tree** - File explorer
- **telescope.nvim** - Fuzzy finder
- **nvim-treesitter** - Syntax highlighting
- **mason.nvim** - LSP package manager
- **dressing.nvim** - Enhanced UI for inputs
- **ollama.nvim** - AI assistance integration
- **avante.nvim** - AI-powered code suggestions (Cursor IDE-style)
- **scnvim** - SuperCollider IDE integration

### LSP & Completion
- **nvim-lspconfig** - LSP configuration
- **mason-lspconfig** - Bridge between mason and lspconfig  
- **nvim-cmp** - Completion engine
- **LuaSnip** - Snippet engine

## Keybindings

### General Navigation
- `Space` - Leader key
- `\` - Local leader key
- `Ctrl + n` - Toggle Neo-tree file explorer
- `Ctrl + p` - Telescope file finder

### AI Assistance
- `<leader>oo` - Open Ollama prompt
- `<leader>oG` - Generate code with Ollama
- `Ctrl + Space` - Trigger AI completions (avante.nvim)

### SuperCollider (scnvim)
- `<M-e>` - Send current line (insert/normal mode)
- `<C-e>` - Send code block or visual selection
- `<Enter>` - Toggle post window
- `<M-CR>` - Toggle post window (insert mode)  
- `<M-L>` - Clear post window
- `<C-k>` - Show function signatures
- `<F12>` - Hard stop SuperCollider
- `<leader>st` - Start SuperCollider
- `<leader>sk` - Recompile class library
- `<F1>` - Server boot (s.boot)
- `<F2>` - Show server meter (s.meter)

### LSP & Diagnostics  
- `K` - Hover documentation
- `gd` - Go to definition
- `gr` - Find references
- `<leader>ca` - Code actions
- `<leader>rn` - Rename symbol  
- `[d`/`]d` - Navigate diagnostics

### Completion Engine
- `Tab`/`Shift+Tab` - Cycle suggestions
- `Ctrl + b/f` - Scroll docs
- `Ctrl + e` - Close completion
- `Enter` - Confirm selection

## Language Support

### Configured Servers
- Lua
- Python  
- Rust
- C/C++
- HTML/CSS
- JSON
- Tailwind CSS
- **SuperCollider** (via scnvim integration)

### Specialized Integration
- **AI Autocomplete**: avante.nvim provides context-aware code suggestions through neural network models
- **Audio Programming**: Full SuperCollider IDE features including:
  - Post window in floating buffer
  - Snippet generation for SC class methods
  - Server status monitoring
  - Interactive help system

## Installation & Setup

1. Clone config:

```
git clone https://github.com/danialrami/nvim-config.git ~/.config/nvim
```


2. Install dependencies:

```
brew install supercollider
cargo install avante-cli
```

3. Start Neovim:

```
nvim
```

## Requirements

- Neovim ≥ 0.9.0
- Nerd Font (icons)
- ripgrep (telescope)
- Ollama local server
- SuperCollider ≥ 3.12
- Rust toolchain (avante.nvim)