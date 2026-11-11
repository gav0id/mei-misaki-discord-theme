[README.md](https://github.com/user-attachments/files/34661176/README.md)

# Mei Misaki — BetterDiscord theme

A rounded Discord theme inspired by **Mei Misaki** (*Another*), with floating panels in the style of the Spotify Discord theme.

- Palette: deep black, bone white, doll-eye blue and crimson.
- Rounded panels, pill-shaped buttons, and rounded menus, embeds and inputs.
- Mei as a background in the chat panel, plus a second image in the Friends tab (both embedded in the file).

![Preview of the Mei Misaki theme]
<img width="1295" height="604" alt="{10216FE9-8E8A-4035-8A7E-37C5257FA5EA}" src="https://github.com/user-attachments/assets/ab539ed1-cd8f-41f9-b5f5-e01b39d682a2" />

## Installation

1. Install [BetterDiscord](https://betterdiscord.app/download) and restart Discord.
2. Download the theme: open `MeiMisaki.theme.css` in this repository and click the **Download raw file** button (the down-arrow icon at the top right of the code viewer). Make sure the file keeps the exact name `MeiMisaki.theme.css`.
3. In Discord: *User Settings → BetterDiscord → Themes → Open Themes Folder*.
4. Copy `MeiMisaki.theme.css` into that folder (on Windows: `%appdata%\BetterDiscord\themes`).
5. Enable **Mei Misaki** in the *Themes* tab. If it doesn't show up, reload with `Ctrl + R`.

## Customization

The variables are at the top of the file, in the `:root` block.

| Variable | What it controls | Default |
|---|---|---|
| `--mei-bg-dim` | Dimming of the chat image (0 = full strength, 1 = invisible) | `0.72` |
| `--mei-bg-position` | Position of the chat image | `right bottom` |
| `--mei-bg-size` | Size of the chat image | `auto 94%` |
| `--mei-friends-dim` | Dimming of the Friends tab image | `0.78` |
| `--mei-friends-position` | Position of the Friends tab image | `38% bottom` |
| `--mei-friends-size` | Size of the Friends tab image | `auto 88%` |
| `--mei-radius` | Corner radius of the panels | `16px` |
| `--mei-gap` | Gap between panels | `8px` |
| `--mei-eye` / `--mei-blood` | Accent colors (blue and crimson) | `#6aaee6` / `#a3263a` |

To use different images, replace the `url(...)` in `--mei-bg-image` or `--mei-friends-image` (the `:root` blocks at the end of the file) with `url("https://...")` or another data URI.

## Notes

- Discord changes its internal class names from time to time, so some elements may stop looking rounded after an update. The selectors use partial matches to reduce this problem.
- The Friends tab image relies on the `:has()` selector, which is available in current Discord versions.
- Using BetterDiscord is against Discord's Terms of Service.
- The images of Mei belong to their respective authors and are used here as personal fan art.
