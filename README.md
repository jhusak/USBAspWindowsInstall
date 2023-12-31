# USBAspWindowsInstall
This simple guide will let you setup USBAsp driver on Windows. Then you can read how to upload hex file to microcontroller/device.

The USBJoy interface has USBAsp programmer built-in. You can activate it by pressing first button DURING connecting USBJoy into USB plug (of course joystick must be connected to USBJoy first).

## Instructions
### Zadig - install usb driver
- Go to http://zadig.akeo.ie/ and download the software (note that Windows XP has a separate link).
- Plug in your USBasp or USBtiny device. In case your microcontroller uses a USBasp or USBtiny bootloader, enter bootloading mode, and let Windows detect the device (it will report driver not found). If a window pops up asking to search for driver, just close it or click on Cancel.
- At this point, run Zadig, it should detect the USBasp or USBtiny, or any libusb device that you have. Then in the selection box (see below), choose libusb-win32 (v1.2.6.0), and click on Install Driver, and wait for the installation to complete.

![Zadig screenshot](/pics/zadig_srceenshot.png)

### Khazama programmer
At http://khazama.com/project/programmer/ you'll find the app.

Here direct link: http://khazama.com/project/programmer/KhazamaAVRProgrammer.rar

You may need WinRar to run the installer.

When installed and run:

1. choose microcontroller "atmega8"

2. load hex file into buffer

3. click the "flash" icon. That's it!

![Khazama screenshot](/pics/khazama.png)

### Congratulations!

Your USBJoy firmware has just been updated!

You may unplug USBJoy and replug it with no keys pressed.
