# Release Notes

## v1.0 — Initial English Translation Release

### Highlights
- **Complete Script & UI Text:** All **4,543** strings across **1,017** text descriptors translated into English, preserving all MG2 control codes (`{BREAK}`, `{END}`, `{NEWLINE}`, `{VAR:XX}`, `{F6:XX}`, `{F7:XXXX}`, `{WAIT:XX}`, `{CTRL:XX}`).
- **Custom English Fonts:** Patched both the 8×16 (`0x385B7C`) and 8×8 outlined (`0x39639C`) 4bpp fonts with lowercase `a`–`z` and English punctuation.
- **English Character Naming Screen:** Replaced the Japanese kana keyboard with an English A–Z / a–z / symbol layout (`0x880000`), updated BG0/BG1 tilemaps, 60-byte keyboard matrix, and 30 default English player names.
- **Deck Setup UI:** Translated the Pre-Dungeon Deck Setup background (`0x66A244` → `0x890000`).
- **Verification:** Verified ROM header/checksum (`0xBD = 0x59`), descriptor/string integrity, Unicorn headless boot & asset transfer, and BPS roundtrip patching.
