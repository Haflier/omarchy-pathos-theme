# Pathos

A minimal Omarchy theme inspired by **philosophy and mathematics** for light mode enjoyers.

![Pathos Preview](preview.png)

## Screenshots

|                           |                           |
| ------------------------- | ------------------------- |
| ![01](screenshots/01.png) | ![02](screenshots/02.png) |
| ![03](screenshots/03.png) | ![04](screenshots/04.png) |
| ![05](screenshots/05.png) | ![06](screenshots/06.png) |


## Installation

```bash
omarchy theme install https://github.com/Haflier/omarchy-pathos-theme.git
```

Then:

```bash
omarchy theme set pathos
```

## Neovim (This is optional for better experience)

Aether has additional internal palette colors that are not exposed through Omarchy's 'colors.toml'. Colors that are not provided by Omarchy fall back to Aether's default palette, which can introduce colors outside the Pathos palette.

You can edit Aether's palette files manually to make Neovim fully match Pathos.

Go inside:
```text
~/.local/share/nvim/lazy/aether/lua/aether/colors/init.lua
```

Then replace ---@class Palette section to this:

```bash
```
---@class Palette
local default_palette = {
	bg = "#000000",
	bg_dark = "#b8b8b8",
	bg_dark1 = "#000000",
	bg_highlight = "#1a1a1a",

	-- Aether accent colors
	blue = "#0747af",
	blue0 = "#264f78",
	blue1 = "#0747af",
	blue2 = "#0747af",
	blue5 = "#0747af",
	blue6 = "#0747af",
	blue7 = "#1e3a5f",

	comment = "#585858",
	cyan = "#0747af",

	dark3 = "#585858",
	dark5 = "#b8b8b8",

	fg = "#d8d8d8",
	fg_dark = "#000000",
	fg_gutter = "#585858", -- Same as base03/comment for visibility

	green = "#1d5419",
	green1 = "#1d5419",
	green2 = "#143811",

	magenta = "#0747af",
	magenta2 = "#f92672",

	orange = "#ff4200",
	purple = "#0747af",

	red = "#f92672",
	red1 = "#c91f4f",

	teal = "#0747af",
	terminal_black = "#282828",

	yellow = "#330694",

	-- Git colors will be calculated from the palette colors above
	git = {},

	-- Base16 compatibility (deprecated, kept for backward compatibility)
	base00 = "#000000",
	base01 = "#282828",
	base02 = "#383838",
	base03 = "#585858",
	base04 = "#000000",
	base05 = "#000000",
	base06 = "#000000",
	base07 = "#f8f8f8",
	base08 = "#f92672",
	base09 = "#ff4200",
	base0A = "#0747af",
	base0B = "#1d5419",
	base0C = "#0747af",
	base0D = "#0747af",
	base0E = "#0747af",
	base0F = "#ff4200",
}
```
```

