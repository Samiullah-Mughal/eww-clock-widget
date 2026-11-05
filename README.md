# Rock Eww

A minimal, aesthetic desktop clock widget built with [Eww](https://github.com/elkowar/eww) for Wayland-based Linux desktops.

Rock Eww brings a clean and elegant touch to your desktop with a stylish date and time display, designed to complement minimal desktop setups.

## Preview

<!-- Add your desktop screenshot here -->
 ![Rock Eww Preview](preview.png) 

## Features

- **Minimal Design** – Clean typography with a distraction-free layout.
- **Live Clock** – Displays the current time with automatic updates every second.
- **Date Display** – Shows the current date and day of the week.
- **Custom Typography** – Uses Anurati and Chilanka fonts for a distinctive look.
- **Wayland Friendly** – Built using Eww for Wayland desktop environments.
- **Lightweight** – Simple configuration with minimal dependencies.

## Built With

- [Eww](https://github.com/elkowar/eww) – Widget framework
- Yuck – Widget configuration
- SCSS – Styling

## Installation

### 1. Install Eww

For Arch Linux and Arch-based distributions:

```bash
yay -S eww
```

### 2. Install Required Fonts

Make sure you have these fonts installed:

- Anurati
- Chilanka

### 3. Clone the Repository

```bash
git clone https://github.com/Samiullah-Mughal/rock-eww.git
```

### 4. Copy Configuration Files

Create the Eww configuration directory if it doesn't exist:

```bash
mkdir -p ~/.config/eww
```

Copy the configuration files:

```bash
cp rock-eww/eww.yuck ~/.config/eww/
cp rock-eww/eww.scss ~/.config/eww/
```

### 5. Launch the Widget

```bash
eww daemon
eww open clock
```

That's it! Your desktop clock should now be running.

## Customization

Want to make it your own?

You can customize the widget by editing:

| File | Purpose |
|---|---|
| `eww.yuck` | Widget structure, data and window configuration |
| `eww.scss` | Colors, fonts, sizes and styling |

After making changes, reload Eww:

```bash
eww reload
```

## Project Structure

```text
rock-eww/
├── eww.yuck
├── eww.scss
└── README.md
```

## Compatibility

Designed for Linux desktops running Wayland with Eww installed.

## Contributing

Suggestions, improvements, and contributions are always welcome!

Feel free to fork the repository and submit a pull request.

## License

See the repository for licensing information.

---

**Made with ❤️ by [Samiullah Mughal](https://github.com/Samiullah-Mughal)**

