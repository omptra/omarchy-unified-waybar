# 📟 Waybar 3: Cyber-Terminal Edition

![Waybar Preview](waybar3.png)

> [!NOTE]
> **Theme Context**: The overall system aesthetic and background shown in the preview is the [Nihil-Omarchy](https://github.com/omptra/Nihil-Omarchy) theme.

## ✨ Vibe & Design
A premium status bar designed for the **Omarchy** / **Hyprland** environment, prioritizing a sharp **cyber-terminal** aesthetic with high-contrast elements and interactive tooltips. This setup features a unique right-side hardware grouping with a horizontal collapsible drawer for a clean yet informative desktop.

- **🎨 Aesthetic**: Solid, high-contrast terminal styling with sharp borders and vibrant neon accents.
- **🌈 Palette**: Deep black (`#0d0d0d`) base with a sharp `#2ac3de` (Cyan) bottom border, `#bb9af7` (Purple) active indicators, and pastel hardware icons.
- **📏 Layout**: 
  - **Left**: Core navigation (OM-Menu, Workspaces, Window Title with smart fallbacks).
  - **Center**: Minimalist time and interactive calendar.
  - **Right**: Media control, essential connectivity (Network/Bluetooth), and a collapsible hardware cabinet.

## 🛠️ Active Modules Breakdown

### 🖱️ Left: Navigation
- **`custom/omarchy`**: Minimalist menu launcher for the Omarchy environment.
- **`hyprland/workspaces`**: Persistent indicators for workspaces 1-5 with smooth animations. **Supports mouse-wheel scrolling!**
- **`hyprland/window`**: Displays current window title, automatically defaulting to "Terminal" when no specific app is active.

### ⏰ Center: Utility
- **`clock`**: Precise time display with a color-coded monthly calendar tooltip on hover/click.

### 📊 Right: System & Media
- **`mpris`**: Dynamic music controls showing track info. Supports scrolling to skip and clicking to play/pause.
- **`network` & `bluetooth`**: Interactive connectivity tiles. Hover for ESSID/Signal strength or connected device battery.
- **`battery`**: Intelligent power monitoring with critical state animations.
- **Horizontal Drawer (``)**: A collapsible cabinet containing `cpu`, `memory`, `temperature`, and `disk` metrics. Clicking CPU/Memory launches a floating `btop` terminal for deep inspection.

## 📦 Prerequisites & Setup

### Fonts 🔠
To render icons and text correctly, please ensure these are installed:
- **[JetBrainsMono Nerd Font](https://github.com/ryanoasis/nerd-fonts)**: Primary system and icon font.
- **Omarchy Custom Font**: Required for the launcher logo.

### Dependencies 📦
For full feature support, install these utilities:
- `waybar` (with Hyprland support)
- `playerctl` (Media control)
- `btop` (System monitoring)
- `omarchy-scripts` (Various custom logic)

## 🚀 How to Apply
1. **Backup**: `mv ~/.config/waybar ~/.config/waybar_backup`
2. **Deploy**: Copy `config.jsonc` and `style.css` to `~/.config/waybar/`.
3. **Reload**: Use the Omarchy reset command or restart manually:
    ```bash
    omarchy-restart-waybar
    ```
    *Manual:* `killall waybar && waybar &`

---
*Part of the [Hyprland Dotfiles](https://github.com/omptra/hyprland-dot-files) collection.*
