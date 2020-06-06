# Hardware Specs

- Gigabyte X570 Aorus Elite
- Ryzen 7 3700X
- Gigabyte 5700XT
- Fenvi wireless adapter

## OpenCore Configuration

- OpenCore 0.5.9
- macOS 10.15.4 (19E287)
- SMBIOS MacPro7,1

## BIOS Configuration

- 4G decoding - Enable

What is not working?
- Sleep

Sleep only works when no USB devices are plugged in.

## Others

### USB

All USB Ports are mapped and corrected.
I removed `ITE Device (8595)` as it was preventing the system from correctly sleeping.

### Boot Args

Without `npci=0x2000`, the screen capture tool (Shift + ctrl + ⌘ + 3) behaves very erratically

### Credits

[Anti](https://amd-osx.com/forum/viewtopic.php?f=35&t=9805) for his inital EFI folder

[barrrrt](https://forum.amd-osx.com/index.php?members/barrrrt.1304/0) for sharing his sleep experience
