# Vectorman Moon + Widescreen (Sega Genesis)

Patches for **Vectorman** (Sega Genesis / Mega Drive, MK-1577, U/E).

- **Moon level:** a new level between Day 12 and the old Day 13.
- **Widescreen (400×224):** optional.

## Downloads (patches/)

| Patch | What it does | Result |
|---|---|---|
| `Vectorman Moon (normal)` | Moon level, normal 320 px | 4 MB |
| `Vectorman Moon (widescreen)` | Moon level + 400 px widescreen | 4 MB |
| `Vectorman Widescreen` | Widescreen only, no moon, original level order | 2 MB |

Each is provided as `.bps` (recommended) and `.ips`. BPS checks that you used the right base ROM; IPS cannot.

## How to patch

You need your own original ROM. This repo contains no game ROM.

- Base ROM: 2,097,152 bytes
- MD5 `d7171a867739c8ec325aa65b175b0c49`
- SHA-1 `57a64d08028b539dc236a693d383f2e1269a5dd4`

Apply **one** patch to the original ROM with Floating IPS, or in a browser at romhacking.net/patch.

Expected results:

| Result | MD5 | SHA-1 |
|---|---|---|
| Moon (normal) | `c91204d8134f3f4353734d64ca5df0fe` | `a7b1a2d0a955e295f31e868d0df270b2e18358dd` |
| Moon (widescreen) | `7f5e9891898ee80af19afdc4d7088630` | `efd0c6ee004fb74f2443758b60d826748e6da7c8` |
| Widescreen only | `ea87fb9c54b4e2f63ff06185536d6d1f` | `44e279268c4dc3696a0e31d7147ac6c3ae27f2dc` |

## Widescreen requirements

Widescreen works **only** in Genesis Plus GX Wide (the libretro core, for example in RetroArch) with the extra columns option set to **10**. It does not work correctly in other emulators. The normal-width moon build runs in standard Genesis emulators.

## Level order (moon builds)

Day 1–12 → **Moon (Day 13)** → Dark Ruins (14) → Underground Vault (15) → Worldlink Center (16) → Twist and Shout (17). Day 1–12 are unchanged.

## Tested

- Rebuilt from source and byte-identical to the released patches.
- 63-check automated suite (layout, boot of every level, death/respawn, checkpoint, laps, level transitions): 0 failures.
- Scripted scans found no CPU exceptions, no writes to ROM or unmapped memory, and no reads of uninitialized RAM across all levels.
- Banners on every level checked against the original.

## Known issues

- Emulator only. Not tested on real hardware or in other emulators.
- Right-edge strip flicker in the Underground Vault and a far-left edge strip in Day 11 in widescreen are known.
- The boss on the 1st level has its wing appear on the edges of the screen.

## Build from source

See `src/`, `widescreen/` and `moon_tests/`. It needs Python 3 (numpy, scipy, Pillow), m68k binutils, and the Genesis Plus GX Wide core.

## Credits

Moon level design, testing and direction: Brandon Hopkins. Built with Claude (Anthropic).
Vectorman © Sega / BlueSky Software. This is an unofficial fan project and is not affiliated with Sega.