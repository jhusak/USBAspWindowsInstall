# USBAspWindowsInstall

Prosta instrukcja, jak zainstalować sterownik USBAsp na Windowsie. Potem możesz przeczytać, jak przesłać plik hex do mikrokontrolera/urządzenia USBJoy.

Interfejs USBJoy ma wbudowany programator USBAsp. Możesz go aktywować, naciskając  przycisk "FIRE" PODCZAS podłączania USBJoy do gniazda USB przez co najmniej 1 sekundę (oczywiście joystick musi być podłączony do USBJoy najpierw).

## Instrukcje

### Zadig - instalacja sterownika USB

- Przejdź na http://zadig.akeo.ie/ i pobierz oprogramowanie (uwaga, Windows XP ma oddzielny link).
- Podłącz urządzenie USBasp lub USBtiny. Jeśli mikrokontroler używa bootloadera USBasp lub USBtiny, przejdź tryb bootloadingu i pozwól systemowi Windows wykryć urządzenie (pokaże komunikat o braku sterownika). Jeśli pojawi się okno z prośbą o wyszukanie sterownika, po prostu zamknij je lub kliknij Anuluj.
- W tym momencie uruchom Zadig, powinien wykryć USBasp lub USBtiny lub jakiekolwiek urządzenie libusb, które masz. Następnie w polu wyboru (patrz poniżej) wybierz libusb-win32 (v1.2.6.0), kliknij Zainstaluj sterownik i czekaj, aż instalacja zostanie zakończona.

![Zrzut ekranu Zadig](/pics/zadig_srceenshot.png)

### Programator Khazama

Na http://khazama.com/project/programmer/ znajdziesz aplikację.

Oto bezpośredni link: http://khazama.com/project/programmer/KhazamaAVRProgrammer.rar

Możesz potrzebować aplikację WinRar, aby uruchomić instalator.

Po zainstalowaniu i uruchomieniu:

1. Wybierz mikrokontroler "atmega8"

2. Wczytaj plik hex do bufora

3. Kliknij ikonę "flash". To wszystko!

![Zrzut ekranu Khazama](/pics/khazama.png)

### Gratulacje!

Firmware USBJoy został właśnie zaktualizowany!

Możesz odłączyć USBJoy i ponownie podłączyć go już bez naciskania żadnych klawiszy.

--------------------------

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
