# Tmux Configuration for Vim Users

This repository contains a productivity-oriented tmux configuration designed to bridge the gap between the terminal and Vim/Neovim. It emphasizes ergonomic movement and intuitive window management.

---

## Core Features

* **Prefix Change**: The default prefix has been moved from `Ctrl+b` to `Ctrl+Space`.
* **Vim-Style Navigation**: Seamless movement between tmux panes and Vim splits using `Ctrl + h/j/k/l`.
* **Intuitive Path Management**: All new windows and panes open in the current working directory.
* **Visual Mode**: A dedicated "Normal Mode" (Copy Mode) that uses Vim keybindings for scrolling and text selection.

---

## Keybindings

### Navigation (No Prefix Required)
These shortcuts work globally across tmux panes and Vim splits.

| Key combination | Action |
| :--- | :--- |
| `Ctrl + h` | Move to the left pane/split |
| `Ctrl + j` | Move to the bottom pane/split |
| `Ctrl + k` | Move to the top pane/split |
| `Ctrl + l` | Move to the right pane/split |

### Pane and Window Management (Prefix: Ctrl + Space)
Press the prefix, release, then hit the following keys.

| Key | Action |
| :--- | :--- |
| `v` | Vertical split (Side-by-side) |
| `h` | Horizontal split (Top-bottom) |
| `n` | Create a new window |
| `m` | Switch to the next window |
| `p` | Switch to the previous window |
| `x` | Close current pane (Immediate) |
| `z` | Zoom pane (Toggle full screen) |
| `r` | Reload tmux configuration |

### Copy Mode (Normal Mode)
Press `Prefix + Escape` to enter.

* Movement: `h`, `j`, `k`, `l`
* Select Text: `v`
* Copy (Yank): `y`
* Exit Mode: `q`

---

## Installation

### 1. Clone the Configuration
Clone this repository into your tmux configuration directory:
```bash
git clone [https://github.com/yourusername/your-repo.git](https://github.com/yourusername/your-repo.git) ~/.config/tmux

```

### 2. Install Tmux Plugin Manager (TPM)

TPM is required to handle the plugins:

```bash
git clone [https://github.com/tmux-plugins/tpm](https://github.com/tmux-plugins/tpm) ~/.tmux/plugins/tpm

```

### 3. Load the Config

If you are already inside tmux, run:

```bash
tmux source ~/.config/tmux/tmux.conf

```

### 4. Install Plugins

Press `Prefix` then `Shift + i` to trigger the TPM installation script.

---

## Required Plugins

The following plugins are used in this setup:

* **tmux-plugins/tpm**: Plugin manager.
* **christoomey/vim-tmux-navigator**: Enables seamless split navigation.
* **catppuccin/tmux**: Mocha flavor theme for the status bar.

