# KL16-FT2232-OpenOCD

## Quick setup

* Download Zadig utility [here](http://zadig.akeo.ie/)
* Use it to install the WinUSB driver to one of the interface of the FT2232 chip
* Install a Telnet client
* Copy the files of this github into the openocd-0.9.0\scripts\ folder
* Edit the start.bat file with the paths that links to your install of openocd and telnet
* Run the bat file with the kinetis KL16 board connected on SWD

## Connection

FTDI |  | Target
--- | --- | ---
1 Vref |  ------------------ | Vcc
4 GND |   ------------------ | GND
5 TDI |   ----470 Ohm---- | SWDIO
9 TCK |   ------------------ | SWCLK
13 TDO |  ------------------ | SWDIO
