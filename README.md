# Shoiko
Rear mounting of electrical components mod for VORON2.4

## What is Shoiko?
Shoiko(背負子)  is an Japanese word meaning "backpack". (naming inspired from [Kirigami](https://github.com/christophmuellerorg/voron_0_kirigami_bed).)

## BOM
Under development: It is a modification of an existing component, but it has never been tested and is "very" experimental. (To be tested soon, but undecided.)
### Main
| Part | Qty | Sourcing | Description/Note |
|---------|-------|----------------| ------------------ |
| din_rail_mount_a | 1 | Print part([STEP](./CAD/din_rail_mount_a.step) or [STL](./STLs/din_rail_mount_a.stl)) |  |
| din_rail_mount_b | 1 | Print part([STEP](./CAD/din_rail_mount_b.step) or [STL](./STLs/din_rail_mount_b.stl)) |  |
| SHCS M3x** | 4 | Local store | TBD |
| M3 Roll-in T-Nut | 4 | [AliExpress](https://www.aliexpress.com/item/32805163712.html) |  |
| 4-wire AWG20 Robot Cable(N meter) | 1 | Local store | Length are TBD. See [Cable Processing](./Docs/cable_processing.md) |
| USB2.0 Type-C Cable | 1 | Local store | See [Cable Processing](./Docs/cable_processing.md) |
| Toolhead PCB | 1 | [AliExpress](https://www.aliexpress.com/item/1005004675264551.html) | AliExpress's link is example for in Stealthburner. |
| BHCS M5x10 | 2 | Local store | Replace of screws due to removal of "XY Cable Chain Bridge". |

### Optional: Corner Brackets
| Part | Qty | Sourcing | Description/Note |
|---------|-------|----------------| ------------------ |
| 2020Frame Corner Bracket 18mmWide | 12 | Print part([STEP](./CAD/2020_CornerBracket_18mm.step) or [STL](./STLs/2020_CornerBracket_18mm.stl)) ||
| SHCS M5x10 | 24 | Local store |  |
| M5 Roll-in T-Nut | 24 | [AliExpress](https://www.aliexpress.com/item/32805163712.html) |  |
| z_belt_cover_a_x2 | 2 | Print part([STEP](./CAD/z_belt_cover_a_x2.step) or [STL](./STLs/z_belt_cover_a_x2.stl)) | Use existing screws and nuts for mounting. |
| z_belt_cover_b_x2 | 2 | Print part([STEP](./CAD/z_belt_cover_b_x2.step) or [STL](./STLs/z_belt_cover_b_x2.stl)) | Use existing screws and nuts for mounting. |

## License
This design are partially derived from the existing Voron parts and hence follow the same License, [GNU GPLv3](https://www.gnu.org/licenses/gpl-3.0.html).
