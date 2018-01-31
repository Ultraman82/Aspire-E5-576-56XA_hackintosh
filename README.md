# Aspire-E5-576-56XA_hackintosh

# [mac osx sierra 10.12.6]
osx version 10.12.6<br>
clover version 4392

# Kexts
ACPIBatteryManager.kext<br>
AppleALC.kext<br>
AppleBacklightInjector.kext<br>
CodecCommander.kext<br>
FakePCIID.kext<br>
FakeSMC.kext<br>
FakePCIID_Intel_HD_Graphics.kext<br>
IntelGraphicsDVMTFixup.kext<br>
IntelGraphicsFixup.kext<br>
Lilu.kext<br>
Shiki.kext<br>
USBInjectAll_patched.kext - <a href="https://github.com/daliansky">daliansky</a><br>
RealtekRTL8111.kext<br>
ApplePS2SmartTouchPad.kext<br>
VoodooI2C.kext<br>
VoodooI2CHID.kext<br>

# Hardware Specification
Acer Aspire E 15 E5-576-56XA<br>

cpu : intel i5-8250u Kaby-Lake-Refresh<br>
ram : ddr3l 4GB + ddr3l 8GB = 12GB 1600Hz<br>
gpu : intel UHD620 8086:5917<br>
lan : Realtek 8411B PCI Express Gigabit Ethernet<br>
cam : UVC Camera VendorID_3034 ProductID_2251<br>
touchpad : ELAN Input Device<br>
wifi : Qualcomm Atheros QCA9377 with Bluetooth nvme - only bluetooth work<br>
sound : Realtek ALC255 Analog<br>

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
5. partially work USB - 480MB (not test USB C Type)
6. audio ALC255, Intel hdmi output work - AppleAlc.kext
7. Internal Display Backlight control. can not control function key.
8. Bluetooth does work. but later replace to BCM94352z.
9. SSD Trim Enable.

# todo
1. SSDT fix
2. when connect hdmi at only first time, internal display is black screen issue.
3. replace wifi/bluetooth card to bcm94352z
4. USB 3.0 nd 3.1
