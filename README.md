# ZainRo Font

Custom fork of the Google Fonts **Zain** typeface created for [bylazar.com](https://bylazar.com). The only modifications are added glyphs for the Romanian characters â, ș, and ț so the site can display Latin content seamlessly.

## Typeface Highlights
- Adds glyphs for Romanian characters â, ș, and ț required by bylazar.com’s Latin copy.
- Ships eight OpenType weights/styles (`Regular`, `Italic`, `Light`, `Light Italic`, `Extra Light`, `Bold`, `Extra Bold`, `Black`).
- Ready for desktop design tools and web embedding via CSS `@font-face`.

## Repository Layout
- `ZainRo/` – compiled desktop and web fonts (`TTF`, `OTF`, `WOFF2`, `EOT`) for immediate use.
- `FontForge/` – editable `.sfd` sources created in FontForge.
- `Original/` – untouched upstream release from Google Fonts plus the SIL Open Font License reference.

## Getting Started
1. **Desktop install (macOS/Windows/Linux)**  
   - Drop the `.ttf` files from `ZainRo/` into your system font manager.  
   - Restart any open design or code tools so they pick up the new family.
2. **Web usage**  
   ```css
   @font-face {
     font-family: "ZainRo";
     src: url("/fonts/ZainRo-Regular.ttf") format("truetype");
     font-weight: 400;
     font-style: normal;
   }
   body { font-family: "ZainRo", "Zain", sans-serif; }
   ```
   Adjust the `src` paths to match your deployment structure and repeat for the other weights/styles you need.

## Building from Source
The FontForge `.sfd` files are the canonical sources.
1. Install [FontForge](https://fontforge.org) (2023 or newer recommended).  
2. Open the desired file from `FontForge/` (e.g., `Zain-Regular.sfd`).  
3. Inspect or modify glyphs as needed.  
4. Generate fonts via `File → Generate Fonts…`, choosing TrueType (`.ttf`) with “Validate Before Saving” enabled.  
5. Replace the corresponding file in `ZainRo/` and verify it on your target platforms.

## License
The project continues to use the SIL Open Font License 1.1 (see `LICENSE.txt`). You may use, modify, and redistribute the fonts as long as you comply with the OFL terms, including preserving the Reserved Font Name “Zain” and “ZainRo”.

## Credits
- Original design: [Google Fonts Zain project](https://github.com/googlefonts/zain)
- Romanian glyph additions: [Myself](https://bylazar.com)
