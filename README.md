# Lenovo-Y70-Hackintosh-OC
Pre-Made EFI folder to boot latest macOS version

Y70-70 OpenCore 0.6.3 macOS 11 Beta Dev 9
Haswell Intel i7-4720HQ / HD 4600

# Remember to edit config.plits "PlatformInfo" section whit GenSMBIOS using this guide from here :
https://dortania.github.io/OpenCore-Install-Guide/config.plist/
# Always using latest Opencore commit downloaded from here :
https://github.com/williambj1/OpenCore-Factory/releases
# Always using latest Kexts Dev Builds downloaded from here :
https://onedrive.live.com/?cid=fe4038da929bfb23&id=FE4038DA929BFB23%21455036&authkey=%21APjCyRpzoAKp4xs

BIOS settings

To start, set BIOS to Windows 8 defaults.

Then insure:

UEFI boot is enabled
secure boot is disabled
enable Legacy Boot (but UEFI first) and you may experience less boot time glitches

Also, be aware that hibernation (suspend to disk or S4 sleep) is not supported on hackintosh.

sudo pmset -a hibernatemode 0
sudo rm /var/vm/sleepimage
sudo mkdir /var/vm/sleepimage

# What's Working
- iGPU / CPU Sensors
- Audio Realtek ALC283 , speakers..
- Touchpad Synaptics
- Intel Wi-Fi whit dedicated "Heliport" app to connect - 2.4Ghz and 20Mhz only low speed under 80Mbps
- Keyboard + Shortcuts like audio (Use Karabiner with windows mode profile)
- Mic And Webcam
- All USB Ports + correct power deliver
- Intel Bluetooth (cannot connect my MX Master Mouse)

# What's Not Working
- GPU - no support for nVidia
- Backlight Keyboard shortcuts
