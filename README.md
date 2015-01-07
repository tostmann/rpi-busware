tostmann/rpi-busware
==========

Linux kernel release 3.12.35-busware+ with builtin busware support for the Raspberry Pi.

Install
-------

```text
sudo REPO_URI=https://github.com/tostmann/rpi-busware rpi-update
```



Changelog
---------
No changes, first release.


Sources
-------
* [raspberrypi/tools](https://github.com/raspberrypi/tools/archive/8f58ab354eac2844c34aeb0e4f19bdb2c96ab99b.tar.gz)
* [raspberrypi/firmware](https://github.com/raspberrypi/firmware/archive/28d2766952d9c603dd96159819fff7bb90aac9cd.tar.gz)
* [raspberrypi/linux](https://github.com/raspberrypi/linux/archive/bac5dc8328a54db970e981f574bd545cae68d7cd.tar.gz)


Patches
--------
None

Kernel config
-------------
Default config: bcmrpi_defconfig



Added:
```text
FB_BACKLIGHT=y
FB_DEFERRED_IO=y
FB_SYS_COPYAREA=y
FB_SYS_FILLRECT=y
FB_SYS_FOPS=y
FB_SYS_IMAGEBLIT=y
FB_TFT=y
FB_TFT_BD663474=m
FB_TFT_FBTFT_DEVICE=m
FB_TFT_HX8340BN=m
FB_TFT_HX8347D=m
FB_TFT_HX8353D=m
FB_TFT_ILI9320=m
FB_TFT_ILI9325=m
FB_TFT_ILI9340=m
FB_TFT_ILI9341=m
FB_TFT_ILI9481=m
FB_TFT_ILI9486=m
FB_TFT_PCD8544=m
FB_TFT_RA8875=m
FB_TFT_S6D02A1=m
FB_TFT_S6D1121=m
FB_TFT_SSD1289=m
FB_TFT_SSD1306=m
FB_TFT_SSD1331=m
FB_TFT_SSD1351=m
FB_TFT_ST7735R=m
FB_TFT_TINYLCD=m
FB_TFT_TLS8204=m
FB_TFT_UPD161704=m
FB_TFT_WATTEROTT=m
GPIO_SX150X=y
RPI_EXT=y
RPI_PIGATOR=y
SERIAL_MAX310X=y
SPI_SC18IS602=y
WIZNET_W5X00=m
```


Changed:
```text
BACKLIGHT_CLASS_DEVICE m -> y
EEPROM_AT24 m -> y
I2C_BCM2708 m -> y
REGMAP_SPI m -> y
SPI_BCM2708 m -> y
```


<p align="center">Built with <a href="https://github.com/notro/rpi-build/wiki">rpi-build</a></p>
