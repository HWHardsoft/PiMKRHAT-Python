# Installation for MKR ENV

![Arduino MKR ENV Shield](https://store-cdn.arduino.cc/uni/catalog/product/cache/1/image/1000x750/f8876a31b63532bbba4e781c30024a0a/a/s/asx00011_iso.jpg)


##  Configuring I2C
```bash
sudo apt-get install -y python-smbus
sudo apt-get install -y i2c-tools
``` 

## Enable I2C Interface
```bash
sudo raspi-config
--> 5 Interfacing Options
--> P5 I2C
--> YES
sudo reboot
``` 

## Testing I2C
```bash
sudo i2cdetect -y 1
```


* replace `xxxxxxxxxxxxxxxxxxxxxxxxx` in  `"WEATHERBIT_IO_KEY": "xxxxxxxxxxxxxxxxxxxxxxxxx"` with your own API key
* replace `de` in `"WEATHERBIT_COUNTRY": "de"` with your country code
* replace `en` in `"WEATHERBIT_LANGUAGE": "en"` with your preferred language
* replace `10178` in `"WEATHERBIT_POSTALCODE": "10178"` with the postal (zip) code of your city (default loaction is Berlin)
* for language-support, please refer to -> **[Weather.io API Docs](https://www.weatherbit.io/api)**

reboot your Pizero!
```bash
sudo reboot
```

