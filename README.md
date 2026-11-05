# Eww Clock Widget

A clean, typography-focused desktop clock widget built with [Eww](https://github.com/elkowar/eww) for Linux desktops running Wayland.

It displays the current day, date, and time in a minimal layout, using Anurati and Chilanka fonts.

## Preview

<!-- Add a screenshot of the widget as preview.png in the repository root. -->
![Eww Clock Widget preview](preview.png)

## Features

- Live clock that refreshes every second
- Day and date display that refresh every minute
- Minimal, centered layout with white typography
- Custom styling with Anurati and Chilanka fonts
- Lightweight configuration using Eww, Yuck, and SCSS

## Requirements

- Linux with a Wayland desktop
- [Eww](https://github.com/elkowar/eww)
- Anurati font
- Chilanka font

## Installation

### 1. Install Eww

On Arch Linux or an Arch-based distribution:

```bash
yay -S eww
```

For other distributions, follow the [official Eww installation guide](https://elkowar.github.io/eww/).

### 2. Install the fonts

Install **Anurati** and **Chilanka** on your system.

### 3. Clone the repository

```bash
git clone https://github.com/Samiullah-Mughal/eww-clock-widget.git
cd eww-clock-widget
```

### 4. Install the configuration

```bash
mkdir -p ~/.config/eww
cp eww.yuck eww.scss ~/.config/eww/
```

### 5. Start the widget

```bash
eww daemon
eww open clock
```

## Customization

Edit the following files inside `~/.config/eww/`:

| File | What it controls |
|---|---|
| `eww.yuck` | Clock data, layout, position, and window behavior |
| `eww.scss` | Fonts, colors, spacing, and text sizes |

After making changes:

```bash
eww reload
```

## Project Structure

```text
eww-clock-widget/
├── eww.yuck
├── eww.scss
└── README.md
```

## Compatibility

Designed for Wayland-based Linux desktops. The window is configured for monitor 0 with a width of 1600px and a top offset of 60px. Adjust the geometry settings in `eww.yuck` to suit your display.

## Contributing

Ideas, bug reports, and improvements are welcome. Feel free to open an issue or submit a pull request.

## License

No license information is currently specified. Add a license file if you want others to know how they may use, modify, and distribute this project.

---

Made by [Samiullah Mughal](https://github.com/Samiullah-Mughal).
