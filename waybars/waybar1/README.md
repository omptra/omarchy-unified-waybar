# 💎 Waybar 1: Omarchy Unified Edition

![Waybar Preview](waybar.png)

> [!NOTE]
> **Theme Context**: The overall system aesthetic and background shown in the preview is the [Nihil-Omarchy](https://github.com/omptra/Nihil-Omarchy) theme.

## ✨ Vibe & Design
A premium, **glassmorphic** status bar designed for the **Omarchy** ecosystem. This setup prioritizes a clean, unified aesthetic with a sharp underline workspace indicator and a dynamic "extra" module drawer to keep your bar minimal yet powerful.

- **🎨 Aesthetic**: Glassmorphic transparency with high-contrast, razor-sharp typography.
- **🌈 Palette**: Deep `#040303` base with a sleek `#aaacac` accent and crisp `#ffffff` foreground.
- **📏 Layout**: 
  - **Left**: Core navigation (Menu, Workspaces, Window Title).
  - **Center**: Time, weather, and system state indicators.
  - **Right**: Media control, essential toggles, and a collapsible system monitor drawer.

## 🚀 Key Features
- **🖼️ Glassmorphism**: Semi-transparent background with subtle border-bottom glow and frosted effects.
- **🔳 Underline Workspaces**: Minimalist icons with a sharp theme-colored underline for the active view.
- **🗃️ Collapsible Drawer**: Keep your bar clean by hiding system metrics (CPU, RAM, Temp, etc.) inside a smooth-transition cabinet.
- **⚡ Live Reload**: Updates style instantly on save—ideal for customization.
- **🕒 Interactive Clock**: Detailed calendar popup with "today" highlighting.

## 🛠️ Active Modules Breakdown

### 🖱️ Left: Navigation
- **`custom/omarchy`**: Minimalist menu launcher for the Omarchy environment.
- **`hyprland/workspaces`**: Unique underline indicators + app icons (Firefox, Kitty, VSCode, etc.). **Supports mouse-wheel scrolling!**
- **`hyprland/window`**: Displays current window title with smart truncation.

### ⏰ Center: Utility
- **`clock`**: Precise 12h time display with a comprehensive calendar popup on click.
- **`custom/weather`**: Real-time updates via `wttrbar` integration.
- **`idle_inhibitor`**: Quick toggle to keep your screen awake (󰈈 / 󰈉).
- **`custom/update`**: Visual notification for pending system updates.

### 📊 Right: Media & Stats
- **`mpris`**: Music controls sharing artist/title info with interactive playback (Left: Play/Pause, Right: Next, Middle: Prev).
- **System Drawer (``)**: A collapsible cabinet containing `cpu`, `memory`, `temperature`, and `disk` usage metrics.
- **Controls**: Interactive icons for Volume, Brightness, and Battery level (with animation for critical battery states).

## 📦 Prerequisites & Setup

### Fonts 🔠
To render icons and text correctly, please ensure these are installed:
- **[JetBrainsMono Nerd Font](https://github.com/ryanoasis/nerd-fonts)**: Primary system font.
- **Symbols Nerd Font**: Icon support.
- **Omarchy Icon Font**: Required for the launcher logo.

### Dependencies 📦
For full feature support, install these utilities:
- `waybar` (with Hyprland support)
- `playerctl` (Media control)
- `brightnessctl` (Backlight)
- `pamixer` (Audio control)
- `swaync` (Notifications)
- `wttrbar` (Weather)

## 🚀 How to Apply
1.  **Backup**: `mv ~/.config/waybar ~/.config/waybar_backup`
2.  **Deploy**: Copy `config.jsonc` and `style.css` to `~/.config/waybar/`.
3.  **Reload**: Use the Omarchy reset command or restart manually:
    ```bash
    omarchy-restart-waybar
    ```
    *Manual:* `killall waybar && waybar &`

---
*Part of the [Hyprland Dotfiles](https://github.com/omptra/hyprland-dot-files) collection.*
