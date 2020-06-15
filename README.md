![title](https://user-images.githubusercontent.com/12926652/73185921-4c3eb580-4162-11ea-863a-d7d973150ecf.png)

# pizero_bikecomputer
a GPS and ANT+ bike computer based on Raspberry Pi Zero (W, WH)

detail in Japanese
https://qiita.com/hishi/items/46619b271daaa9ad41b3

Disclaimer : Instructions in English have been slightly trimmed and roughly translated from the link above using DeepL.

# Table of Contents

- [Abstract](#abstract)
- [Features](#features)
- [Parts list](#Part-list)
- [Assembly](#assembly)
- [Installation](#installation)
- [Quick Start](#quick-start)
- [Usage](#usage)
- [Comparison with other bike computers](#comparison)
  - [Overview](#overview)
- [Q&A](#qa)


...

comming soon!


# Abstract

![image](https://qiita-user-contents.imgix.net/https%3A%2F%2Fqiita-image-store.s3.ap-northeast-1.amazonaws.com%2F0%2F100741%2Fa6746d2f-bae0-a511-f6e7-972d4c6bc592.png?ixlib=rb-1.2.2&auto=format&gif-q=60&q=75&w=1400&fit=max&s=a8197e8537ebdd4fcd490776442855c7)

# Comparison

- 200km ride with Garmin Edge 830 and Pizero Bikecomputer ([strava activity](https://www.strava.com/activities/2834588492))

![title-03.png](https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/100741/b355cb92-8e7f-6b3f-7cd0-98ba8803a56c.png)

| Items | Edge830 | Pi Zero Bikecomputer |
|:-:|:-:|:-:|
| Distance | 193.8 km  | 194.3 km  |
| Work |  3,896 kJ | 3,929 kJ  |
| Moving time | 9:12 | 9:04  |
| Total Ascent | 2,496 m | 2,569 m |


# Hardware list / Part list
 * Raspberry Pi Zero [W](https://www.kubii.fr/cartes-raspberry-pi/1851-raspberry-pi-zero-w-kubii-3272496006997.html) [11€] or  [WH](https://www.kubii.fr/cartes-raspberry-pi/2076-raspberry-pi-zero-wh-kubii-3272496009394.html) [14€] ), for setup, see the author's article (jp) ["Setting up the Raspberry Pi Zero (W, WH)"](https://qiita.com/hishi/items/8bdfd9d72fa8fe2e7573) etc.
 * [TFT LCD module with touch screen PiTFT 2.4"](https://www.digikey.fr/products/fr?keywords=%201528-2048-ND%20) recommended [32€], on [adafruit](https://www.adafruit.com/product/2455), for setup, see the author's article (jp) ["Using PiTFT with Raspberry Pi Zero (W, WH)"](https://qiita.com/hishi/items/bdd630666277e4f8162a), it is assumed that you are able to view X Window.
 * GPS module [Akizuki Denshi's modules](http://akizukidenshi.com/catalog/g/gK-09991/) ~17€ are probably the best way to get started, it uses the MT3339 chip which is supported by GPSd. Setup is described below...**add details about more readily available GPS modules**
 * ANT+ USB dongle [ANTUSB-m](https://www.digikey.fr/product-detail/fr/garmin-canada-inc/ANTUSB-M/1094-1009-ND/3947399) ~19€, you'll also need a [Tiny OTG Adapter - USB Micro to USB](https://www.digikey.fr/products/fr?keywords=%201528-1597-ND%20) ~3€, to plug the dongle onto the Pi Micro USB port.
 * I2C sensor(s), this bike computer was initially developped with an Enviro pHAT, but it has been since discontinued...**to be developped/clarified**
 * [Pimoroni Button SHIM](https://www.digikey.fr/products/fr?keywords=%201528-2402-ND%20) *no stock on Digikey*, on [adafruit](https://www.adafruit.com/product/3582).
 * [PiJuice](https://uk.pi-supply.com/products/pijuice-standard). **non visible on the pictures**
 * [PiJuice Zero](https://uk.pi-supply.com/products/pijuice-zero). **non visible on the pictures**
 * Right angle Micro USB cable **add link to product**
 * Powerbank (3000 mAh should last 8 hours with the PiTFT version).
 * Screws and nuts (M2.5), used to secure to differents boards together, some 6mm long and some 15-20mm long **to be detailled**
 * SD card, whatever you have on hand (8GB or bigger). If you use it every week, it will die after about a year. The original author is currently using the SanDisk high endurance version of the 32GB and it's been good for a year now.
 * Soldering Iron, solder
 * Jumper wires and lead wires
 * Insulation tape (cellophane tape, etc.)
 * Wire cutters.
 
# License

This repository is available under the [GNU General Public License v3.0](https://github.com/hishizuka/pizero_bikecomputer/blob/master/LICENSE)

# Author

[hishizuka](https://github.com/hishizuka/) ([@pi0bikecomputer](https://twitter.com/pi0bikecomputer) at twitter)
