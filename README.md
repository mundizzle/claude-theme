# Claude Theme

A color theme aligned with Anthropic's official brand palette. Available for VS Code and Ghostty terminal.

![Claude Theme Dark](.github/images/claude-dark.png)
![Claude Theme Light](.github/images/claude-light.png)

## Features

- Colors match Anthropic's official brand palette (Orange, Blue, Green on warm neutrals)
- Light and dark variants
- Consistent colors across VS Code and Ghostty terminal

## Accent Palette

| Role | Hex | Color |
|------|-----|-------|
| Keywords | `#d97757` | Orange (brand) |
| Strings | `#788c5d` | Green (brand) |
| Links | `#6a9bcc` | Blue (brand) |
| Functions / Numbers | `#c08c3a` | Amber |
| Types | `#6a9b91` | Teal |
| Variables | `#9588a8` | Lavender |
| Error | `#DC2626` | Red |

## Background Colors

### Light Theme
| Color | Hex | Usage |
|-------|-----|-------|
| Warm Cream | `#faf9f5` | Main background |
| White | `#ffffff` | Cards, inputs |
| Light Gray | `#e8e6dc` | Borders, dividers |
| Primary Text | `#141413` | Body text |

### Dark Theme
| Color | Hex | Usage |
|-------|-----|-------|
| Dark | `#141413` | Main background |
| Elevated | `#262624` | Cards, panels |
| Deep | `#0a0a09` | Inputs |
| Primary Text | `#faf9f5` | Body text |

## VS Code Installation

### Option 1: Symlink (recommended for development)

```bash
# macOS/Linux
ln -s /path/to/claude ~/.vscode/extensions/claude

# Windows (PowerShell as Admin)
New-Item -ItemType SymbolicLink -Path "$env:USERPROFILE\.vscode\extensions\claude" -Target "C:\path\to\claude"
```

### Option 2: Copy

```bash
# macOS/Linux
cp -r /path/to/claude ~/.vscode/extensions/

# Windows
xcopy /E /I "C:\path\to\claude" "%USERPROFILE%\.vscode\extensions\claude"
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
cp ghostty/claude-* ~/.config/ghostty/themes/
```

Add to `~/.config/ghostty/config`:

```
# Single theme
theme = claude-dark

# Or auto-switch with system appearance
theme = dark:claude-dark,light:claude-light
```

Restart Ghostty to apply.

## License

MIT License - see [LICENSE](LICENSE) for details.
