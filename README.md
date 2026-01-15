# Claude Theme

A warm, elegant color theme inspired by Claude's aesthetic. Available for VS Code and Ghostty terminal.

## Features

- Warm, eye-friendly color palette based on Claude's UI
- No blue colors - uses warm amber and teal alternatives
- Both light and dark variants
- Consistent colors across VS Code and Ghostty terminal

## Claude Cowork Color Reference

### Light Theme

| # | Category | Color | Hex | Usage |
|---|----------|-------|-----|-------|
| 1 | Background | Cream White | `#FFFCF9` | Main background |
| 2 | Background | Warm White | `#FAF7F4` | Sidebar, secondary |
| 3 | Background | Light Beige | `#F5F1ED` | Cards, chips |
| 4 | Background | Pure White | `#FFFFFF` | Inputs |
| 5 | Border | Subtle | `#E7E5E4` | Dividers |
| 6 | Border | Input | `#D6D3D1` | Form borders |
| 7 | Border | Grid | `#F0ECE8` | Subtle lines |
| 8 | Text | Primary | `#1F1D1B` | Headings, body |
| 9 | Text | Secondary | `#57534E` | Descriptions |
| 10 | Text | Muted | `#78716C` | Placeholder |
| 11 | Text | Subtle | `#A8A29E` | Disabled, icons |
| 12 | Accent | Terracotta | `#D97757` | Buttons, links |
| 13 | Accent | Hover | `#C4684A` | Button hover |
| 14 | Semantic | Error | `#DC2626` | Error text |
| 15 | Semantic | Warning | `#D97706` | Warning text |
| 16 | Semantic | Success | `#059669` | Success, strings |
| 17 | Syntax | Functions | `#B8860B` | Function names |
| 18 | Syntax | Types | `#3D8B80` | Types, classes |
| 19 | Syntax | Variables | `#7C3AED` | Variables |
| 20 | Syntax | Numbers | `#D97706` | Numeric values |

### Dark Theme

| # | Category | Color | Hex | Usage |
|---|----------|-------|-----|-------|
| 1 | Background | Charcoal | `#2D2926` | Main background |
| 2 | Background | Elevated | `#332E2A` | Cards, panels |
| 3 | Background | Chip | `#3A3530` | Chips, hover |
| 4 | Background | Deep | `#1F1B18` | Inputs, recessed |
| 5 | Border | Subtle | `#3A3530` | Dividers |
| 6 | Border | Card | `#443F3A` | Card borders |
| 7 | Border | Input | `#3D3833` | Form borders |
| 8 | Text | Primary | `#F5F1ED` | Headings, body |
| 9 | Text | Secondary | `#D6D3D1` | Descriptions |
| 10 | Text | Muted | `#A8A29E` | Placeholder |
| 11 | Text | Subtle | `#78716C` | Disabled, icons |
| 12 | Accent | Terracotta | `#D97757` | Buttons, links |
| 13 | Accent | Hover | `#E8896B` | Button hover |
| 14 | Semantic | Error | `#EF4444` | Error text |
| 15 | Semantic | Warning | `#FBBF24` | Warning text |
| 16 | Semantic | Success | `#34D399` | Success, strings |
| 17 | Syntax | Functions | `#E9A23B` | Function names |
| 18 | Syntax | Types | `#5EADA4` | Types, classes |
| 19 | Syntax | Variables | `#A78BFA` | Variables |
| 20 | Syntax | Numbers | `#FBBF24` | Numeric values |

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
