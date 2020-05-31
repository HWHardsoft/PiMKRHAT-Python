# Installation for MKR RGB

![Arduino MKR RGB Shield](https://store-cdn.arduino.cc/uni/catalog/product/cache/1/image/1000x750/f8876a31b63532bbba4e781c30024a0a/a/s/asx00010_iso.jpg)

A good starting point for own experiments with the RGB shield is the [APA102 library](https://github.com/tinue/apa102-pi) by tinue. We are using software SPI because the pins of the Arduino MKR RGB shield are not connected to the SPI interface of the Raspberry Pi. 

## Install APA102
```bash
sudo apt install python-pip3
sudo pip3 install apa102-pi
```
