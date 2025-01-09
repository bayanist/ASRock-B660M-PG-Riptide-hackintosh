# ASRock-B660M-PG-Riptide-AlderLake

## User's Hardware Specification

| Component              | Model / Specification                                     | Hackintosh Compatibility |
|------------------------|-----------------------------------------------------------|--------------------------|
| **Motherboard**        | ASROCK B660M PG Riptide (BIOS Version: 11.05 |              ✅ OK                    |
| **Processor**          | Intel Core i5-12400F                                      | ✅ OK                    |
| **CPU Cooler**         | DEEPCOOL AK400 ZERO DARK PLUS                             | ✅ OK                    |
| **RAM**                | Patriot Viper Steel 32Gb DDR4 4133MHz (PVS416G413C9K)     | ✅ OK                    |
|                        | (4x8Gb KIT)                                               |                          |
| **GPU**                | Sapphire AMD Radeon RX 6600 XT                            | ✅ OK                    |
| **Audio**              | 7.1 CH HD Audio (Realtek ALC897 Audio Codec)              | ✅ OK (using VoodooHDA)  |
| **Storage 1**          | Crucial 500GB M.2 (CT500P5PSSD8)                          | ✅ OK                    |
| **Storage 2**          | KingSpec SSD 256GB (OS: Windows 10)                       | ✅ OK                    |
| **Storage 3**          | Seagate ST500DM002-1BD142 (HDD, 500GB)                    | ✅ OK                    |
| **Power Supply**       | MONTECH BETA 650                                          | ✅ OK                    |
| **Network Card**       | Intel Wi-Fi 6E AX210                                      | ✅ OK (with kexts)       |
| **Bootloader**         | OpenCore 1.0.3                                            | ✅ OK                    |

---

## SSDT Table

| Path                   | Comment                                                    | Enabled |
|------------------------|------------------------------------------------------------|---------|
| **SSDT-ALSO.aml**      | Ambient Light Sensor Device                                | ✅ true |
| **SSDT-PLUG-ALT.aml**  | Redefines CPU Objects as Processor                         | ✅ true |
| **SSDT-RTCAWAC.aml**   | Context-Aware AWAC Disable and RTC Enable/Fake/Range Fix   | ✅ true |
| **SSDT-MCHC.aml**      | Memory Controller Hub                                      | ✅ true |
| **SSDT-USBX.aml**      | Generic USBX device for USB power properties               | ✅ true |
| **SSDT-SBUS.aml**      | System Management Bus (SMBus) K                            | ✅ true |
| **SSDT-EC.aml**        | Embedded Controller (EC)                                   | ✅ true |
| **SSDT-Bridge.aml**    | Create missing PCI bridges for passed device path          | ✅ true |
| **SSDT-PMC.aml**       | Enables Native VRAM on True 300-Series Boards              | ✅ true |


### Notes:
- All components are confirmed to work on Hackintosh with **macOS Sonoma 14.7.2 (23H311)**.
- **Audio**: Realtek ALC897 works using `VoodooHDA` for sound output and input.
- **Bootloader**: OpenCore 1.0.3 is used for system boot and configuration.
- Intel Wi-Fi 6E AX210 requires additional **kexts** for full functionality.
- GPU and other components operate smoothly on macOS Sonoma.