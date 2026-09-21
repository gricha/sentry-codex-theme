# Sentry Dusk & Dawn

Two quiet Codex desktop themes based on Sentry’s website colors. Muted surfaces, restrained purple accents, readable text, and opaque windows.

| Theme | Appearance | Import string | Preview |
| --- | --- | --- | --- |
| **Dusk** | Dark charcoal plum and soft off-white text | [sentry-dusk.codex-theme.txt](sentry-dusk.codex-theme.txt) | [preview.html](preview.html) |
| **Dawn** | Soft lavender-white and dark violet text | [sentry-dawn.codex-theme.txt](sentry-dawn.codex-theme.txt) | [preview-light.html](preview-light.html) |

## Import into Codex

1. Open the theme’s `.txt` file and copy its entire contents, including `codex-theme-v1:`. GitHub’s **Raw** view provides the plain text.
2. Open **Settings → Appearance** in Codex. Appearance may be under General in some versions.
3. Choose **Import** in the matching section: **Dark theme** for Dusk or **Light theme** for Dawn.
4. Paste the share string and select **Import theme**.
5. Select the matching appearance mode to see it.

The light and dark importers reject a share string for the opposite appearance mode.

The app’s preset label remains **Sentry** for Dusk and **GitHub** for Dawn. The installed Sentry syntax preset supports dark mode only, so Dawn uses GitHub Light syntax with custom Sentry interface colors. The share format does not define a custom preset name or custom syntax tokens.

## Preview locally

Clone or download this repository, then open `preview.html` or `preview-light.html` in a browser. The links at the top switch between versions. **Select import string** selects the complete payload; press **⌘C** on macOS or **Ctrl+C** on Windows to copy it.

The previews illustrate the palette and approximate the app layout. They use flat surfaces without drop shadows, inset shadows, glow, or a colored selection edge. The imported theme controls colors, contrast, fonts, and window opacity; it does not replace the app’s CSS.

## Palette

| Role | Dusk | Dawn |
| --- | --- | --- |
| Background | `#211D2B` | `#F6F5F8` |
| Text | `#ECECF1` | `#362D59` |
| Accent | `#6A5FC1` | `#6A5FC1` |
| Added code | `#7DB6A0` | `#31765F` |
| Removed code | `#E1567C` | `#C73852` |
| Skills | `#C4A7CB` | `#8C5393` |
| Contrast setting | 46 / 100 | 40 / 100 |
| Primary text contrast | 14.0:1 | 11.5:1 |

Both themes use default fonts and opaque windows. The backgrounds, green addition colors, and Dusk’s skill color are adaptations; the remaining palette values come directly from Sentry’s website.

## Sources and compatibility

Colors were researched on September 21, 2026, from [Sentry’s branding page](https://sentry.io/branding/) and its [live stylesheet](https://sentry.io/_astro/Layout.D-BjuX0r.css). Relevant tokens include:

- `--color-rich-black`: `#1F1633`, the reference for Dusk’s desaturated background.
- `--color-dk-violet`: `#362D59`.
- `--color-blurple`: `#6A5FC1`.
- `--color-gray-2`: `#ECECF1`.
- `--color-md-pink`: `#E1567C`.
- `--color-dk-pink`: `#C73852`.
- `--color-md-purple`: `#8C5393`.

[Official appearance documentation](https://learn.chatgpt.com/docs/reference/settings#appearance) describes custom colors and theme sharing. Both payloads were accepted by the installed app’s share-string parser and theme schema; their code presets were checked for the matching appearance variant. The previews were visually checked. A live app import was not performed.
