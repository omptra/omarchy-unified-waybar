# 🌌 Omarchy: Hyprland Dotfiles

<p align="center">
  <img src="https://raw.githubusercontent.com/catppuccin/catppuccin/main/assets/palette/macchiato.png" width="400" />
  <br />
  <b>A premium, glassmorphic ricing experience for Omarchy OS.</b>
  <br />
  <i>Elegance in every pixel, speed in every keybinding.</i>
</p>

---

## 🛠 Overview

Welcome to my personal collection of **Hyprland** configuration files, specifically tailored for **Omarchy OS**. This repository is designed to provide a unified, aesthetic, and highly functional desktop environment that balances minimalism with power-user utility.

Whether you're looking for a sharp, glassmorphic Waybar or a fully optimized Hyprland workflow, you'll find the building blocks of my Omarchy rice here.

---

## 📸 Showcase

> [!TIP]
> ### 🚧 Screenshots Coming Soon!
> I'm currently fine-tuning the final animations and layout. The full desktop rice is so "premium" that even the screenshot tool is shy. Check back soon for a visual feast of the "Omarchy" experience! 🎨✨

---

## 📂 Directory Structure

| Directory | Description |
| :--- | :--- |
| [📂 `waybars/`](./waybars) | A curated collection of unique Waybar themes (Omarchy Unified, Floating Bliss, etc.) |
| `📂 hyprland/` | Core Hyprland config files, window rules, and keybindings. *(Coming Soon)* |
| `📂 scripts/` | Custom utility scripts for volume, brightness, and system management. |
| `📂 assets/` | Wallpapers, icons, and fonts used across the configurations. |

---

## 🚀 Installation & Setup

### 1. Prerequisites
Before applying these dots, ensure you are running **Omarchy OS** (or any Arch-based system) and have the following installed:

*   **WM**: `hyprland-git`
*   **Bar**: `waybar`
*   **Launcher**: `rofi-wayland` or `wofi`
*   **Notifications**: `swaync`
*   **Terminals**: `kitty` or `foot`
*   **Shell**: `zsh` (with Oh-My-Zsh & Powerlevel10k recommended)

### 2. Required Fonts 🔠
These configurations rely heavily on specific Nerd Fonts to render icons correctly:
- **[JetBrainsMono Nerd Font](https://github.com/ryanoasis/nerd-fonts)** (Primary)
- **Symbols Nerd Font** (Icons)
- **Omarchy Icon Font** (Internal assets)

### 3. Applying the Configs
To get started, clone the repository and symlink the desired components to your `.config` directory:

```bash
# Clone the repository
git clone https://github.com/omptra/hyprland-dot-files.git
cd hyprland-dot-files

# Example: Applying Waybar1
mkdir -p ~/.config/waybar
ln -sf $(pwd)/waybars/waybar1/config.jsonc ~/.config/waybar/config
ln -sf $(pwd)/waybars/waybar1/style.css ~/.config/waybar/style.css
```

---

## 🛠 Features

- **Glassmorphic UI**: High transparency with background blur and sharp borders.
- **Dynamic Drawers**: Collapsible system monitors to keep the workspace clean.
- **Unified Palette**: Harmonious colors designed for the Omarchy ecosystem.
- **Optimized for Speed**: Extremely low latency keybindings and animations.
