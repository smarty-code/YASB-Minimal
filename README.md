# YASB Minimal Theme

A clean, minimal configuration for [YASB](https://github.com/amnweb/yasb) (Yet Another Status Bar) for Windows.

![Theme Preview](https://img.shields.io/badge/YASB-Minimal-blue?style=flat-square)

## Features

- **Minimal Design** - Clean, distraction-free status bar
- **Blur Effect** - Translucent background with rounded corners
- **System Monitoring** - CPU and Memory usage widgets
- **Weather Integration** - Real-time weather with custom icons
- **Network Traffic** - Upload/download speed monitoring
- **Calendar Popup** - Interactive calendar with week numbers
- **Volume Control** - Quick access to sound settings

## Widgets

| Widget | Position | Description |
|--------|----------|-------------|
| Windows Button | Left | Opens start menu |
| CPU | Left | CPU usage percentage |
| Memory | Left | RAM usage percentage |
| Clock | Center | Time, date, and calendar |
| Weather | Right | Current temperature and conditions |
| Volume | Right | System volume control |
| Traffic | Right | Network speed monitor |
| Recycle Bin | Right | Bin status and quick actions |

## Installation

1. Install [YASB](https://github.com/amnweb/yasb)
2. Copy `config.yaml` and `styles.css` to your YASB config directory:
   ```
   %USERPROFILE%\.config\yasb\
   ```
3. Restart YASB

## Configuration

### Weather API
Update the `api_key` in the weather widget section of `config.yaml`:
```yaml
weather:
  options:
    api_key: "YOUR_API_KEY"
    location: "Your City, Country"
```

Get a free API key from [WeatherAPI](https://www.weatherapi.com/).

### Timezone
Modify the timezone in the clock widget:
```yaml
clock:
  options:
    timezones: ["Your/Timezone"]
```

## Font Requirements

This theme uses **JetBrainsMono Nerd Font** for icons. Install it from:
- [Nerd Fonts](https://www.nerdfonts.com/font-downloads)

## Color Palette

| Color | Hex | Usage |
|-------|-----|-------|
| Primary Text | `#cdd6f4` | Main text and icons |
| Secondary Text | `#8b9cb0` | Dimmed elements |
| Accent Blue | `#89dceb` | Clock and highlights |
| Accent Red | `#f38ba8` | Alarm indicators |
| Background | `#909fb215` | Widget backgrounds |

## File Structure

```
YASB-Minimal/
├── config.yaml    # Widget configuration
├── styles.css     # Theme styling
└── README.md      # Documentation
```

## Customization

### Changing Colors
Edit the color values in `styles.css`. Main colors are defined in the base styles section.

### Adding/Removing Widgets
Modify the `widgets` section under `bars.primary-bar` in `config.yaml`:
```yaml
widgets:
  left: ["win_button", "cpu", "memory"]
  center: ["clock"]
  right: ["weather", "volume", "traffic", "bin"]
```

## Author

**Smarty Code** - [@smarty-code](https://github.com/smarty-code)

Created with ❤️ for the Windows customization community.

## License

MIT License - Feel free to modify and share.

## Credits

- Theme designed by [Smarty Code](https://github.com/smarty-code)
- [YASB](https://github.com/amnweb/yasb) by amnweb
- [Catppuccin](https://github.com/catppuccin) color inspiration
