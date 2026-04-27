# Claude Theme

A color theme aligned with Anthropic's official brand palette. Available for VS Code, Ghostty terminal, Zed, and Codex.

![Claude Theme Dark](.github/images/claude-dark.png)
![Claude Theme Light](.github/images/claude-light.png)

## Features

- Colors match Anthropic's official brand palette (Orange, Blue, Green on warm neutrals)
- Light and dark variants
- Consistent colors across VS Code, Ghostty terminal, and Zed
- Codex app theme import strings

## Palette

Official Anthropic brand anchors:

| Role | Hex | Color |
|------|-----|-------|
| Primary Accent | `#d97757` | Orange |
| Secondary Accent | `#6a9bcc` | Blue |
| Tertiary Accent | `#788c5d` | Green |
| Dark | `#141413` | Primary text and dark backgrounds |
| Light | `#faf9f5` | Light backgrounds and text on dark |
| Mid Gray | `#b0aea5` | Secondary elements |
| Light Gray | `#e8e6dc` | Subtle backgrounds |

Supporting syntax colors:

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

## Zed Installation

```bash
# Create themes directory
mkdir -p ~/.config/zed/themes

# Copy theme family file
cp zed/claude.json ~/.config/zed/themes/
```

Restart Zed or reopen the theme selector, then select **Claude Light** or **Claude Dark**.

Zed also supports mode-based theme selection in `~/.config/zed/settings.json`:

```json
{
  "theme": {
    "mode": "system",
    "light": "Claude Light",
    "dark": "Claude Dark"
  }
}
```

## Codex Installation

The Codex app uses share strings for importing Appearance themes. The Claude themes in `codex/` follow the app's `codex-theme-v1:` import format and keep the built-in Codex code theme selected.

### Import Light Theme

1. Open Codex Settings
2. Go to **Appearance**
3. Under **Light theme**, choose **Import**
4. Paste the contents of `codex/claude-codex-light.txt`
5. Choose **Import theme**

### Import Dark Theme

1. Open Codex Settings
2. Go to **Appearance**
3. Under **Dark theme**, choose **Import**
4. Paste the contents of `codex/claude-codex-dark.txt`
5. Choose **Import theme**

The readable source payloads and generated share strings live in `codex/claude-codex-theme.json`.

## License

MIT License - see [LICENSE](LICENSE) for details.
