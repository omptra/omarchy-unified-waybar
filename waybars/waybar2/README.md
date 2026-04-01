![Waybar 2 Screenshot](waybar2.png)

> [!NOTE]
> **Theme Context**: The system theme visible in the background is [Nihil-Omarchy](https://github.com/omptra/Nihil-Omarchy). Follow the link for more details!

# 🌌 Waybar 2: Floating Catppuccin Islands

Welcome to the **Waybar 2** configuration—a premium, aesthetic, and functional status bar designed for the **Omarchy OS** / **Hyprland** environment. This setup moves away from the traditional solid bar in favor of a modern "pilled" island design with glassmorphism effects.

## ✨ Aesthetic & Layout
Unlike the standard continuous bar, **Waybar 2** utilizes a **three-island layout**:
- **Floating Pills**: Each module group is encased in a semi-transparent, rounded capsule (`border-radius: 20px`) that appears to float at the top of the monitor.
- **Catppuccin Mocha Palette**: A curated color scheme featuring soft pastels (Blue, Green, Yellow, Flamingo) on a deep, dark background.
- **Glassmorphism**: Subtle box shadows and `0.95` opacity backgrounds provide a premium "frosted glass" feel.
- **Dynamic Workspaces**: Workspaces don't just show numbers; they dynamically display icons for the applications currently running on them.

## 🛠️ Modules Breakdown
### 🖱️ Left Island: Navigation
- **Launcher**: A custom "omarchy" branded icon to trigger your application menu.
- **Workspaces**: Minimalist icons (󰖟, , ) that change color based on activity, with smooth transitions and persistent indicators for the first 5 desktops. **Supports mouse-wheel scrolling!**

### ⏰ Center Island: Time
- **Clock & Calendar**: Clean digital clock that reveals a detailed calendar and month view on click/hover.

### 📊 Right Island: System Tray & Stats
- **MPRIS**: Media controls and track information (Artist - Title) with play/pause interaction.
- **System Drawer (``)**: A collapsible container that hides/shows advanced system metrics (CPU usage, Memory, Temp, Disk) to keep the bar clean.
- **Network & Bluetooth**: Minimalist status symbols (Wi-Fi and Bluetooth) that stay out of the way until needed.
- **Controls**: Interactive icons for Volume, Brightness, and Battery level (with animation for critical battery states).
- **Tray**: Standard system tray for app indicators.

## 📦 Dependencies & Fonts
To ensure all icons and functionalities work correctly, please install the following:

### Fonts 🔠
- **JetBrainsMono Nerd Font**: The primary font for text and symbols.
- **Omarchy Custom Font**: Required for the launcher logo.

### Packages 📦
- `waybar-hyprland` (or `waybar` with Hyprland support)
- `playerctl`: For music information and control.
- `brightnessctl`: For brightness scrolling and display.
- `swaync`: For the notification center integration.
- `btop`: Triggered when clicking on CPU/Memory stats.
- `wiremix` / `pulseaudio`: For audio management.

## 🚀 How to Switch
To apply this setup to your Omarchy environment:

1.  **Backup** your current waybar config: `mv ~/.config/waybar ~/.config/waybar_backup`
2.  **Symlink** this directory: `ln -s /path/to/waybar2 ~/.config/waybar`
3.  **Reload** Hyprland or restart waybar using the custom command:
    ```bash
    omarchy-restart-waybar
    ```
    *Alternatively, manual reload:*
    ```bash
    killall waybar && waybar &
    ```
4.  Alternatively, update your `hyprland.conf` to point to this directory:
    ```ini
    exec-once = waybar -c ~/.config/waybar/config.jsonc -s ~/.config/waybar/style.css
    ```

---
*Created for the Omarchy Community.*
