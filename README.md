# tool_i3_display

Brightness and monitor layout helpers for an i3/X11 desktop.

## Commands

- `brup` - increase laptop brightness
- `brdown` - decrease laptop brightness
- `monitors-brightness` - show/set DDC monitor brightness
- `monitors-init` - apply the saved three-monitor layout
- `monitors-on` - enable secondary monitors
- `monitors-off` - disable secondary monitors

## Dependencies

- bash
- brightnessctl
- xrandr
- i3-msg
- ddcutil
- i3status (optional)

## Install

```bash
./install.sh
```

Install to a custom prefix:

```bash
PREFIX="$HOME/.local" ./install.sh
```

## Usage

```bash
brup
brdown
monitors-brightness
monitors-brightness 75
monitors-init
```

## Configuration

- Set `MONITORS="1 2 3"` for monitors-brightness.
- Set `I3STATUS_ADDITIONAL_CMD` to refresh extra i3status text.

## Notes

These scripts were extracted from a personal Arch Linux + i3 workspace. Review dependencies and paths before using them on another machine.
