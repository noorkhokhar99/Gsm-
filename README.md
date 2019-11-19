# Gsm-
Serial Communication in Raspberry Pi 3


Open the LX teminal and type:

dmesg | grep tty

The list will show, ttyS0 – UART corresponding to the GPIO header.

To operate the GPIO UART at the correct baud rate, enter sudo nano /boot/config.txt in the terminal and add the two lines

core_freq=250

enable_uart=1

Save the file and reboot the Pi.
