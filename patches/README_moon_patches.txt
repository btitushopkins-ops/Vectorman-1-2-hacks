Vectorman - Moon Level (extra level between Day 12 and the old Day 13, shown as "Day 13 / Moon")

Patch these onto an unmodified Vectorman (Genesis, U/E, MK-1577) ROM:
  size 2,097,152 bytes, header checksum 0xE039
  MD5  d7171a867739c8ec325aa65b175b0c49
  SHA1 57a64d08028b539dc236a693d383f2e1269a5dd4
The result is a 4 MB ROM.

  Vectorman Moon (normal).bps/.ips      - normal 320x224 build (any emulator / flash cart*)
  Vectorman Moon (widescreen).bps/.ips  - 400x224 widescreen build, ONLY for Genesis Plus GX Wide
                                          (libretro core, set the extra columns option to 10)

Use the .bps files if you can (Flips, beat, MultiPatch ...): they check the base ROM and the result, so a wrong
ROM is refused instead of silently producing a broken game. The .ips files are the same patches for tools that
only know IPS (IPS cannot check anything). Apply ONE of the two builds, not both.
You must supply your own original ROM; no game data is distributed here except the bytes the patches contain.

Expected result of patching:
  normal      MD5 4145c43ddc001633aaa26048257fe6dc  SHA1 7bef5cb05cd0a394ffc34dc87a88de5cfbe5557c  (4,194,304 bytes)
  widescreen  MD5 b244a3d786eace950b03b78fee5714f8  SHA1 4cf005e8834fa7d2bcad68dba10a49be740d82c6  (4,194,304 bytes)

Level order: ... Day 12 -> Moon ("Day 13") -> Dark Ruins ("Day 14") -> Underground Vault ("Day 15")
-> Worldlink Center ("Day 16") -> Twist and Shout ("Day 17"). Day 1-12 are unchanged.

* Tested only in emulators (Genesis Plus GX family). Not tested on real hardware. See KNOWN_ISSUES.md.
