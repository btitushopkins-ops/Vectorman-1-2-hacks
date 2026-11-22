Vectorman - Widescreen (400x224), no other changes

Patch onto an unmodified Vectorman (Genesis, U/E, MK-1577) ROM:
  size 2,097,152 bytes, header checksum 0xE039
  MD5  d7171a867739c8ec325aa65b175b0c49
  SHA1 57a64d08028b539dc236a693d383f2e1269a5dd4
Result is still 2 MB (header checksum 0x62B3).
  MD5 ea87fb9c54b4e2f63ff06185536d6d1f  SHA1 44e279268c4dc3696a0e31d7147ac6c3ae27f2dc

Works ONLY on Genesis Plus GX Wide (libretro core, extra columns option set to 10).
Level order, banners and transitions are exactly the original game's.
Prefer the .bps file (it verifies the base ROM and the result); the .ips is for tools that only read IPS.
This patch contains no data copied from the original game.
