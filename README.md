# USBAspWindowsInstall
This simple guide will let you setup USBAsp driver on Windows. Then you can read how to upload hex file to microcontroller/device.

## Instructions

- Go to http://zadig.akeo.ie/ and download the software (note that Windows XP has a separate link).
- Plug in your USBasp or USBtiny device. In case your microcontroller uses a USBasp or USBtiny bootloader, enter bootloading mode, and let Windows detect the device (it will report driver not found). If a window pops up asking to search for driver, just close it or click on Cancel.
- At this point, run Zadig, it should detect the USBasp or USBtiny, or any libusb device that you have. Then in the selection box (see below), choose libusb-win32 (v1.2.6.0), and click on Install Driver, and wait for the installation to complete.

![Zadig screenshot](/pics/zadig_screenshot.png)
