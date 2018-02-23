# Aspire-E5-576-56XA_hackintosh

# [mac osx sierra 10.12.6]
osx version 10.12.6<br>
clover version 4392

# references
1. <a href="https://github.com/RehabMan/OS-X-Clover-Laptop-Config">OS-X-Clover-Laptop-Config</a>
2. <a href="https://www.reddit.com/r/hackintosh/comments/7amizy/guide_installing_macos_high_sierra_on_the_mi/">guide_installing_macos_high_sierra_on_the_mi</a>
# Kexts
[EFI/CLOVER/kexts/Other]
ACPIBatteryManager.kext<br>
AppleALC.kext<br>
CodecCommander.kext<br>
FakeSMC.kext<br>
FakePCIID.kext<br>
FakePCIID_Intel_HD_Graphics.kext<br>
FakePCIID_Broadcom_WiFi.kext<br>
IntelGraphicsDVMTFixup.kext<br>
IntelGraphicsFixup.kext<br>
Lilu.kext<br>
Shiki.kext<br>
BrcmPatchRAM2.kext<br>
RealtekRTL8111.kext<br>
ApplePS2SmartTouchPad.kext<br>
VoodooI2C.kext<br>
VoodooI2CHID.kext<br>

[Library/Extensions]
AppleBacklightInjector.kext<br>

[System/Library/Extensions]
BrcmPatchRAM2.kext<br>
BrcmFirmwareRepo.kext<br>

# Hardware Specification
Acer Aspire E 15 E5-576-56XA<br>

cpu : intel i5-8250u Kaby-Lake-Refresh<br>
ram : ddr3l 4GB + ddr3l 8GB = 12GB 1600Hz<br>
gpu : intel UHD620 8086:5917<br>
lan : Realtek 8411B PCI Express Gigabit Ethernet<br>
cam : UVC Camera VendorID_3034 ProductID_2251<br>
touchpad : ELAN Input Device<br>
wifi : Qualcomm Atheros QCA9377 -> Broadcom BCM94352Z<br>
sound : Realtek ALC255 Analog<br>
lcd : LM156LF1L03<br>

Intel(R) Xeon(R) E3 - 1200 v6/7th Gen Intel(R) Core(TM) Host Bridge/DRAM Registers - 5914<br>
Intel(R) Serial IO I2C Host Controller - 9D60<br>
Mobile 6th/7th Generation Intel(R) Processor Family I/O PCI Express Root Port #9 - 9D18<br>
Mobile 6th/7th Generation Intel(R) Processor Family I/O PCI Express Root Port #12 - 9D1B<br>
Mobile 6th/7th Generation Intel(R) Processor Family I/O PCI Express Root Port #11 - 9D1A<br>
Mobile 6th/7th Generation Intel(R) Processor Family I/O PMC - 9D21<br>
Mobile 6th/7th Generation Intel(R) Processor Family I/O SMBUS - 9D23<br>
Mobile 6th/7th Generation Intel(R) Processor Family I/O Thermal subsystem - 9D31<br>
Mobile 7th Generation Intel(R) Processor Family I/O LPC Controller (U with iHDCP2.2 Premium) - 9D4E<br>

# working
1. UHD620 Internal Display, HDMI - fake ig-platform-id & fake IntelGFX
2. when connect hdmi at only first time, internal display is black screen.
3. when internal display black, if lid closed and open work dual display.
4. Touch Pad, Keyboard
5. audio ALC255, Intel hdmi output work - AppleAlc.kext
6. Internal Display Backlight control. can not control function key.
7. BCM94352z WiFi & Bluetooth.
8. SSD Trim Enable.

# todo
1. SSDT / DSDT fix (working...)
2. when connect hdmi at only first time, internal display is black screen issue.

