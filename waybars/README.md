# 🎨 Waybar Gallery: Omarchy OS Collection

Welcome to the official gallery of **Waybar** themes for the **Omarchy OS** / **Hyprland** ecosystem. This repository serves as a showcase of meticulously crafted status bars, ranging from minimalist glassmorphic panels to modern floating islands.

Each configuration is designed to be functional, aesthetic, and fully integrated with the Omarchy design language.

---

## 🖼️ Gallery

Explore the different designs available in this collection. Click on the headings to jump into the specific theme's directory for detailed documentation and code.

### 🍱 [Waybar 1: Omarchy Unified Edition](./waybar1)
> *A premium, glassmorphic panel with a sharp underline workspace indicator and a dynamic module drawer.*

![Waybar 1 Preview](./waybar1/waybar.png)

- **Vibe**: Glassmorphism, Unified, Professional.
- **Highlights**: Dynamic "extra" drawer, underline workspace indicators, high-contrast typography.

---

### 🌌 [Waybar 2: Floating Catppuccin Islands](./waybar2)
> *A modern "pilled" island design featuring the iconic Catppuccin Mocha palette.*

![Waybar 2 Preview](./waybar2/waybar2.png)

- **Vibe**: Floating Pills, Soft Pastels, Modern.
- **Highlights**: Three-island layout, application-aware workspace icons, frosted glass effects.

---

### 💻 [Waybar 3: Cyber-Terminal Edition](./waybar3)
> *A premium, sharp terminal aesthetic with interactive tooltips and a collapsible hardware drawer.*

![Waybar 3 Preview](./waybar3/waybar3.png)

- **Vibe**: Cyber-Terminal, Sharp, Functional.
- **Highlights**: Collapsible horizontal hardware drawer, interactive color-coded calendar, high-contrast cyan/purple palette.

---


## 🚀 How to Swap Themes

Swapping between these themes is straightforward. Follow these steps to apply a new look to your Hyprland setup:

### 1. Backup your current configuration
Before making changes, it's always a good idea to back up your existing Waybar setup.
```bash
mv ~/.config/waybar ~/.config/waybar_backup
```

### 2. Choose and Link a Theme
Navigate to this directory in your terminal and create a symbolic link to the theme you want to use. Replace `waybarX` with your choice (e.g., `waybar2`).

```bash
# Example: Using Waybar 2
ln -s $(pwd)/waybar2 ~/.config/waybar
```

### 3. Reload Waybar
Restart Waybar to see the changes immediately.
```bash
killall waybar && waybar &
```

> [!NOTE]
> **Omarchy OS** users can simply run `omarchy-restart-waybar` to reload the bar.

> [!TIP]
> If you want to switch back, simply remove the symlink and restore your backup:
> `rm ~/.config/waybar && mv ~/.config/waybar_backup ~/.config/waybar`

---

## 🛠️ General Prerequisites
While each theme may have specific needs, most rely on:
- **Fonts**: [JetBrainsMono Nerd Font](https://github.com/ryanoasis/nerd-fonts), Symbols Nerd Font.
- **Tools**: `playerctl`, `brightnessctl`, `pamixer`, `swaync`, `btop`.

*Part of the [Hyprland Dotfiles](https://github.com/omptra/hyprland-dot-files) collection.*
