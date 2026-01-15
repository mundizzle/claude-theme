# Claude Theme

A warm, elegant color theme inspired by Claude's aesthetic. Available for VS Code and Ghostty terminal.

## Features

- Warm, eye-friendly color palette based on Claude's UI
- No blue colors - uses warm amber and teal alternatives
- Both light and dark variants
- **Unified accent palette** - same syntax colors in both themes (inspired by Solarized)
- Consistent colors across VS Code and Ghostty terminal

## Design Philosophy

Inspired by [Solarized](https://ethanschoonover.com/solarized/), this theme uses a **unified accent palette** - the same 8 syntax highlighting colors work on both light and dark backgrounds. This provides:

- Consistent color meanings when switching themes
- Colors chosen for medium brightness (readable on any background)
- Reduced eye strain through selective contrast

## Unified Accent Palette

These 8 colors are shared between light and dark themes:

| Role | Hex | Color |
|------|-----|-------|
| Keywords | `#D97757` | Terracotta |
| Strings | `#7A937A` | Sage |
| Functions | `#B38B2D` | Amber |
| Types | `#4A9B92` | Teal |
| Variables | `#9080B0` | Lavender |
| Numbers | `#C08830` | Gold |
| Error | `#DC2626` | Red |
| Comments | `#78716C` | Stone |

## Background Colors

### Light Theme
| Color | Hex | Usage |
|-------|-----|-------|
| Cream White | `#FFFCF9` | Main background |
| Warm White | `#FAF7F4` | Sidebar |
| Light Beige | `#F5F1ED` | Cards |
| Primary Text | `#1F1D1B` | Body text |

### Dark Theme
| Color | Hex | Usage |
|-------|-----|-------|
| Charcoal | `#2D2926` | Main background |
| Elevated | `#332E2A` | Cards, panels |
| Deep | `#1F1B18` | Inputs |
| Primary Text | `#F5F1ED` | Body text |

## VS Code Installation

### Option 1: Symlink (recommended)

```bash
# macOS/Linux
ln -s /path/to/claude-theme ~/.vscode/extensions/claude-theme

# Windows (PowerShell as Admin)
New-Item -ItemType SymbolicLink -Path "$env:USERPROFILE\.vscode\extensions\claude-theme" -Target "C:\path\to\claude-theme"
```

### Option 2: Copy

```bash
# macOS/Linux
cp -r /path/to/claude-theme ~/.vscode/extensions/

# Windows
xcopy /E /I "C:\path\to\claude-theme" "%USERPROFILE%\.vscode\extensions\claude-theme"
```

### Activate

1. Open VS Code
2. Press `Cmd+K Cmd+T` (macOS) or `Ctrl+K Ctrl+T` (Windows/Linux)
3. Select **Claude Light** or **Claude Dark**

## Ghostty Installation

```bash
# Create themes directory
mkdir -p ~/.config/ghostty/themes

# Copy theme files
cp ghostty/claude-light ~/.config/ghostty/themes/
cp ghostty/claude-dark ~/.config/ghostty/themes/
```

Add to `~/.config/ghostty/config`:

```
theme = claude-dark
```

Restart Ghostty to apply.

## License

MIT License - see [LICENSE](LICENSE) for details.
