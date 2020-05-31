# Installation for MKR THERM

![Arduino MKR THERM Shield](https://store-cdn.arduino.cc/uni/catalog/product/cache/1/image/1000x750/f8876a31b63532bbba4e781c30024a0a/a/s/asx00012_iso.jpg)


##  Install smbus library
```bash
sudo apt-get install -y python-smbus
sudo apt-get install -y i2c-tools
``` 

## Install additional libraries
This program requires the Adafruit Python MAX31855 library:

```bash
sudo apt install python-pip3
sudo pip3 install adafruit-circuitpython-max31855
```
