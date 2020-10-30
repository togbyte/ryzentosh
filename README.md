# OSX on Intel & AMD
I have been a fan of Hacintosh for number years. I built several custom PCs running OSX from those "Lion" days.

I would like to share some of builds and configuration with those who are interested doing the same. Have fun!!!


Asus X570-I | Ryzen 3950X | Sapphire 5700XT | G.Skill 32GB 
- Awesome watercooled monster Ryzentosh I built over the Covid-19 pandemic days
- Tested and Working OS
  - Big Sur 11.0.1
  - Catalina 10.15.5+
  - Mojave 10.14
  - Windows 10
- Overclocked CPU to 4.3Ghz at 1.3VCore: Geek Benchmark 1310 / 15334.  Cinebench R20: 10248+
  - X570-I Bios 2606
  - DOCP enabled
  - Disabled FastBoot, SecureBoot, CFG
- OpenCore 0.6.1
  - Require RebuildAppleMemoryMap = True and SetupVirtualMap = False
  - Add device: PciRoot(0x0)/Pci(0x8,0x1)/Pci(0x0,0x4)
    Set layout-id = 7
- Kexts
  - AMDRyzenCPUPowerManagement 0.6.5
  - AppleALC 1.5.2
  - SmallTreeIntel82576 1.0
  - VirtualSMC 1.1.6
  - WhateverGreen 1.4.2
- USB Port Mapped
- WIFI / Bluetooth
  - Replaced with BCM94360NG 802.11AC Bluetooth 4.0
