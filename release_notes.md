# Release Notes

## v1.0.1 — English Translation Release

### Changes in v1.0.1
- **Compact BPS Patch (`TargetCopy`):** Reduced `monster_gate_2_en.bps` from ~8.4 MB to **423 KB** (`423,051` bytes) by encoding repeated `0xFF` expansion padding with BPS `TargetCopy`, improving compatibility and load speed on web and mobile patchers while producing the exact same target ROM (`CRC32: E0246534`).
- **Level-Clear Graphic:** Translated the level-clear `カード獲得` OAM sprite (`0x2A7124`–`0x2A7924`) to **`CARD GET!`** in the matching chrome-horizon style.

## v1.0.0 — English Translation Release

### Highlights
- **Complete Script & UI Text:** All **4,543** strings across **1,017** text descriptors translated into English, preserving all MG2 control codes (`{BREAK}`, `{END}`, `{NEWLINE}`, `{VAR:XX}`, `{F6:XX}`, `{F7:XXXX}`, `{WAIT:XX}`, `{CTRL:XX}`), with full line-wrapping and box-fit alignment (including `desc 13` Dungeon Advice, `desc 249` Dungeon Escape, and `desc 8/854..858` Character Select).
- **Custom English Fonts:** Patched both the 8×16 (`0x385B7C`) and 8×8 outlined (`0x39639C`) 4bpp fonts with lowercase `a`–`z` and English punctuation, plus `MICRO_FONT_3x7` for Card HUD/List name sprites.
- **English Character Naming Screen:** Replaced the Japanese kana keyboard with an English A–Z / a–z / symbol layout (`0x880000`), updated BG0/BG1 tilemaps, OAM labels, 60-byte keyboard matrix, and 30 default English player names.
- **Full UI & Card Graphics:** Translated 107 unique Card HUD/List 4bpp name sprites (`0x72CDC0`–`0x72D914`), 6 Opening Intro slides, Character Select buttons & difficulty pills, Mode Menu & Badges, Deck Setup, Option, Link, Data Select, 11 Town banners & menus, Guild Menu & Quest headers, Card Categories, Monster Book, Shop, Dungeon Pause, Dungeon `ADVICE` tab, and level-clear `CARD GET!` sprite (`0x2A7124`–`0x2A7924`), plus `Yes/No` cursor spacing fixes.
- **Verification:** Verified ROM header/checksum (`0xBD = 0x59`, `CRC32: E0246534`), 100% binary descriptor/string decode, whole-ROM unindexed descriptor scan, Unicorn headless boot & asset transfers, live `mGBA` gameplay captures, and BPS/IPS roundtrip patching.
