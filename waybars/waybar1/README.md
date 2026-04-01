# Waybar: Omarchy Unified Edition

![Waybar Preview](waybar.png)

> [!NOTE]
> **Theme Context**: The overall system aesthetic and background shown in the preview is the [Nihil-Omarchy](https://github.com/omptra/Nihil-Omarchy) theme.

## Overview
A premium, glassmorphic Waybar configuration designed for the **Omarchy** ecosystem. This setup prioritizes a clean, unified aesthetic with a sharp underline workspace indicator and a dynamic "extra" module drawer to keep your bar minimal yet powerful.

## Vibe & Design
- **Aesthetic**: Glassmorphic transparency with high-contrast typography.
- **Palette**: Dark `#040303` base with a sleek `#aaacac` accent and crisp `#ffffff` foreground.
- **Layout**: 
  - **Left**: Core navigation (Menu, Workspaces, Window Title).
  - **Center**: Time, weather, and system state indicators.
  - **Right**: Media control, essential toggles, and a collapsible system monitor drawer.

## Active Modules
- **Navigation**: `custom/omarchy` (Menu), `hyprland/workspaces`, `hyprland/window`
- **Utility**: `idle_inhibitor`, `clock`, `custom/weather` (via `wttrbar`), `custom/update` indicator.
- **Media**: `mpris` control with artist/title display.
- **Hardware**: `backlight`, `pulseaudio` (In/Out), `network`, `bluetooth`, `battery`.
- **Drawer (Extra)**: A collapsible cabinet containing `cpu`, `memory`, `temperature`, `disk` usage, and `custom/notification`.

## Prerequisites

### Required Fonts
To render icons and text correctly, you need:
- **[JetBrainsMono Nerd Font](https://github.com/ryanoasis/nerd-fonts)**
- **Symbols Nerd Font**
- **Omarchy Icon Font** (Repository specific)

### Dependencies
Ensure these utilities are installed for full functionality:
- `waybar` (with Hyprland support)
- `playerctl` (Media control)
- `brightnessctl` (Backlight)
- `pamixer` (Audio control)
- `swaync` (Notifications)
- `wttrbar` (Weather)
- `btop` (System monitoring)
- `omarchy-scripts` (Various custom logic)

## Installation
1. Copy `config.jsonc` and `style.css` to your `~/.config/waybar/` directory.
2. Ensure you have the required fonts installed.
3. Reload Waybar using `omarchy-restart-waybar` or manually with `killall waybar && waybar &`.

---
*Part of the [Hyprland Dotfiles](https://github.com/omptra/hyprland-dot-files) collection.*
