# Waybar: Cyber-Terminal Style (Omarchy Re-sync Edition)

![Waybar Preview](waybar3.png)

> [!NOTE]
> **Theme Context**: The overall system aesthetic and background shown in the preview is the [Nihil-Omarchy](https://github.com/omptra/Nihil-Omarchy) theme.

## Overview
A premium, highly customized Waybar configuration prioritizing a sharp terminal aesthetic with interactive tooltips and a logical right-side grouping featuring a horizontal hardware drawer.

## Vibe & Design
- **Aesthetic**: Solid, high-contrast terminal styling with interactive tooltips and custom animations.
- **Palette**: Deep black (`#0d0d0d`) base with a sharp cyan (`#2ac3de`) bottom border, purple (`#bb9af7`) highlights for active states, and pastel greens/reds for hardware.
- **Layout**: 
  - **Left**: Core navigation (Menu, Workspaces, Window Title).
  - **Center**: Time and Calendar.
  - **Right**: Media control, Network, Bluetooth, Battery, and a collapsible hardware drawer.

## Active Modules
- **Navigation**: `custom/omarchy` (Menu), `hyprland/workspaces` (Persistent 1-5, scroll-to-switch), `hyprland/window` (Rewrites empty titles to "Terminal").
- **Utility**: `clock` (Interactive color-coded monthly calendar tooltip).
- **Media**: `mpris` (Dynamic artist/title, scroll-to-skip, click-to-pause).
- **Hardware**: `network` (Hover for ESSID/Signal strength), `bluetooth` (Shows connected device alias & battery %), `battery` (Blinking animation on critical).
- **Drawer**: A collapsible horizontal cabinet containing `cpu`, `memory`, `temperature`, and `disk`. Clicking CPU/Memory launches a floating `btop` terminal.

## Prerequisites

### Required Fonts
To render icons and text correctly, you need:
- **[JetBrainsMono Nerd Font](https://github.com/ryanoasis/nerd-fonts)**
- **Omarchy Icon Font** (Repository specific)

### Dependencies
Ensure these utilities are installed for full functionality:
- `waybar` (with Hyprland support)
- `playerctl` (Media control)
- `btop` (System monitoring)
- `omarchy-scripts` (Various custom logic)

## Installation
1. Copy `config.jsonc` and `style.css` to your `~/.config/waybar/` directory.
2. Ensure you have the required fonts installed.
3. Reload Waybar using `omarchy-restart-waybar` (or `killall waybar && waybar &`).

---
*Part of the [Hyprland Dotfiles](https://github.com/omptra/hyprland-dot-files) collection.*
