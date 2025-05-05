# Development Environment Configuration

A comprehensive configuration setup for a modern development environment, featuring Neovim, Tmux, and various terminal utilities optimized for efficiency and productivity.

## 🚀 Overview

This repository contains dotfiles and configurations for creating a cohesive development environment with the following core components:

- **Neovim**: A highly extensible text editor with modern IDE capabilities
- **Tmux**: Terminal multiplexer for session management
- **Zathura**: A minimalist document viewer
- **Foot**: A fast, lightweight Wayland terminal emulator
- **FastFetch**: A fast system information tool

## 📦 Core Components

### 1. Neovim Configuration

The Neovim setup is built with a modular architecture using Lua:

#### Plugin Management

- Uses `lazy.nvim` for efficient plugin management
- Lazy-loading support for optimal startup time

#### Key Features

- **LSP Integration**: Comprehensive language server support with:
  - Diagnostics
  - Code completion
  - Symbol navigation
  - Code actions
- **Development Tools**:
  - Treesitter for advanced syntax highlighting
  - Telescope for fuzzy finding
  - Harpoon for quick file navigation
  - DAP for debugging support
  - Flutter tools for mobile development
- **Code Quality**:

  - Built-in formatting support
  - Linting integration
  - Git integration via Fugitive

- **UI Enhancements**:
  - Gruvbox theme
  - Zen mode for focused editing
  - Custom status line
  - File tree navigation

### 2. Tmux Configuration

Optimized for seamless integration with Neovim:

- Custom key bindings for efficient pane/window management
- Mouse support enabled
- Status bar positioned at top
- Vim-style navigation
- Session management capabilities
- Gruvbox theme integration

### 3. Terminal Utilities

#### Zathura

- PDF viewer with vim-like keybindings
- Gruvbox theme integration
- Custom statusbar configuration

#### Foot Terminal

- Modern terminal emulator
- JetBrains Mono Nerd Font integration
- Gruvbox theme
- Custom padding and transparency settings

#### FastFetch

- Customized system information display
- Organized into hardware, software, and system sections
- Custom ASCII art integration

## 🛠 Installation

1. Clone the repository:

```bash
git clone https://github.com/renamice/config.git ~/.config
```

2. Install required dependencies:

```bash
# Neovim dependencies
sudo apt-get install ripgrep

# Install language servers and tools via Mason
:MasonInstall clangd lua_ls rust_analyzer html cssls svelte emmet_ls
```

3. Set up Tmux plugin manager:

```bash
git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
```

## ⌨️ Key Bindings

### Neovim

- Leader key: `Space`
- `<leader>ff`: Find files
- `<leader>fg`: Live grep
- `<leader>gs`: Git status
- `<leader>zm`: Toggle Zen mode
- `<leader>u`: Toggle Undotree

### Tmux

- Prefix: `Ctrl + Space`
- `prefix + l`: Split horizontally
- `prefix + j`: Split vertically
- `prefix + h/j/k/l`: Navigate panes
- `M-H/L`: Switch windows

## 🎨 Themes

The environment uses the Gruvbox theme consistently across all components:

- Neovim: Gruvbox with custom transparency options
- Tmux: Gruvbox-styled status bar
- Zathura: Gruvbox color scheme
- Foot: Gruvbox terminal colors

## 🔧 Customization

- All configurations are modular and can be easily modified
- Each component's settings are separated into logical files
- Clear documentation within configuration files
- Consistent styling across all tools

## 📝 Contributing

1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Create a new Pull Request
