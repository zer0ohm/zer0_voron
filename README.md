# zer0_voron
## About zer0_voron
A repository for compiling modified parts, or a [hashtag](https://twitter.com/search?q=%23zer0_voron) to be added to tweets about VORON.

## BOM
Under development: It is a modification of an existing component, but it has never been tested and is "very" experimental. (To be tested soon, but undecided.)
### Shoiko(背負子)
 * Rear mounting of electrical components mod for VORON2.4
 * din_rail_mount_a/b inspired from [SnakeOil-XY](https://github.com/SnakeOilXY/SnakeOil-XY/blob/master/BETA2_Release/STLs/Panels/Back-panel/Bottom/4x_din-holder.stl)
 
| Part | Qty | Sourcing | Description/Note |
|---------|-------|----------------| ------------------ |
| din_rail_mount_x2 | 2 | Print part([STEP](./CAD/din_rail_mount_x2.step) or [STL](./STLs/din_rail_mount_x2.stl)) |  |
| SHCS M3x** | 2 | Local store | Length are TBD. |
| M3 Roll-in T-Nut | 2 | [AliExpress](https://www.aliexpress.com/item/32805163712.html) |  |
| SB2040 Cable-harness <br> or <br> 2-wire 18AWG Robot Cable(3 meter) + 2-wire AWG22 Robot Cable(3 meter) | 1 | [AliExpress](https://www.aliexpress.com/item/1005004819126687.html) <br> or <br> [Misumi(AWG18)](https://jp.misumi-ec.com/vona2/detail/222000262826/?HissuCode=%EF%BE%9B%EF%BE%8E%EF%BE%9E%EF%BE%84%EF%BD%AF%EF%BE%8C%EF%BE%9FDPC3+AWG18X2C-3) + <br> [Misumi(AWG22)](https://jp.misumi-ec.com/vona2/detail/222000262826/?HissuCode=%EF%BE%9B%EF%BE%8E%EF%BE%9E%EF%BE%84%EF%BD%AF%EF%BE%8C%EF%BE%9FDPC3+AWG22X2C-3)| Length are TBD. See [Cable Processing](./Docs/cable_processing.md) |
| RJ11 Cable | 1 | [Misumi](https://jp.misumi-ec.com/vona2/detail/110500076440/?HissuCode=CBLRJ050-666-S-07-SV) | For BTT Octopus only. See [Cable Processing](./Docs/cable_processing.md) |
| Toolhead PCB | 1 | [AliExpress](https://www.aliexpress.com/item/1005004675264551.html) | AliExpress's link is example for in Stealthburner. |
| BHCS M5x10 | 2 | Stock or Local store | Replace of screws due to removal of "XY Cable Chain Bridge". |

### Modified Corner Brackets
 * Attempt to determine if printed brackets can be used to strengthen rigidity
 * model based Misumi's HBLFSN5(2mm narrower to avoid interference with Z_Idler)

| Part | Qty | Sourcing | Description/Note |
|---------|-------|----------------| ------------------ |
| 2020Frame Corner Bracket 18mmWide | 12 | Print part([STEP](./CAD/2020_CornerBracket_18mm.step) or [STL](./STLs/2020_CornerBracket_18mm.stl)) ||
| SHCS M5x10 | 24 | Local store |  |
| M5 Roll-in T-Nut | 24 | [AliExpress](https://www.aliexpress.com/item/32805163712.html) |  |
| z_belt_cover_a_x2 | 2 | Print part([STEP](./CAD/z_belt_cover_a_x2.step) or [STL](./STLs/z_belt_cover_a_x2.stl)) | Use existing screws and nuts for mounting. |
| z_belt_cover_b_x2 | 2 | Print part([STEP](./CAD/z_belt_cover_b_x2.step) or [STL](./STLs/z_belt_cover_b_x2.stl)) | Use existing screws and nuts for mounting. |

### XYEndstop PCB for X_Carriage
 * Endstop PCB utilizing the switch mounting holes on the back side of X_Carriage 

| Part | Qty | Sourcing | Description/Note |
|---------|-------|----------------| ------------------ |
| Endstop PCB | 1 | order PCB yourself([KiCad](./)) or [Single item PCB from me](https://zer0ohm.booth.pm/) ||
| Self-tapping screw M2x12 or M2x14 | 2 | Local store or [AliExpress](https://www.aliexpress.com/item/1005002306042593.html) | PCB mount screw |
| D2F-L3-A1 microswitch | 1 | Digikey or Mouser or Local store | X Endstop |
| D2F-L3 microswitch | 1 | Digikey or Mouser or Local store | Y Endstop |
| JST-XH S3B-XH-A | 1 | Digikey or Mouser or Local store |  |
| JST XH XHP-3 | 1 | Digikey or Mouser or Local store | Qty is the number used on this PCB only, the number may vary depending on the connection point. |

### Front Skirt PowerUI Mod(for 350mm build only)
 * Mod to bring "inlet and switch"(PowerUI) to front skirt
 * Can divert parts used in existing front_skirt_a and power_inlet_filtered

| Part | Qty | Sourcing | Description/Note |
|---------|-------|----------------| ------------------ |
| front_skirt_a_mod | 1 | Print part([STEP](./CAD/front_skirt_a_mod.step) or [STL](./STLs/front_skirt_a_mod.stl)) ||
| [Optional] power_inlet_filtered_mod | 1 | Print part([STEP](./CAD/power_inlet_filtered_mod.step) or [STL](./STLs/power_inlet_filtered_mod.stl)) | Optional part. May use original parts. |

## Klipper_Configs
* Config for BTT Octopus+Mellow SB2040
* based [VORON's config](https://github.com/VoronDesign/Voron-2/blob/Voron2.4/firmware/klipper_configurations/Octopus/Voron2_Octopus_Config.cfg) and [Mellow/KlipperCN's config](https://mellow.klipper.cn/#/board/fly_sb2040/cfg)

| File | Description/Note |
|------|------------------|
| printer.cfg | |
| steppers.cfg | XYZ motor drive settings |
| toolhead.cfg | SB2040 settings |
| octopus_heatmanage.cfg | Bed-heater and FAN(excl toolhead fans) control |
| neopixel.cfg | lighting settings in chamber |
| macros.cfg | |
| display.cfg | BTT Mini12864 settings |

## What is Shoiko?
Shoiko(背負子)  is an Japanese word meaning "backpack". (naming inspired from [Kirigami](https://github.com/christophmuellerorg/voron_0_kirigami_bed).)

## License
This design are partially derived from the existing Voron parts and hence follow the same License, [GNU GPLv3](https://www.gnu.org/licenses/gpl-3.0.html).
