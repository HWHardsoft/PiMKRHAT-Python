# PiMKRHAT Python code examples
Python examples for Arduino MKR bridge HAT](https://www.hwhardsoft.de/english/projects/pimkrhat) for Raspberry Pi and different Arduino MKR shields.

![PiMKRHAT and MKR ENV Shield](https://user-images.githubusercontent.com/3049858/83356701-0e4bdb00-a368-11ea-8c06-ff7c251af9ee.jpg)

![PiMKRHAT](https://user-images.githubusercontent.com/3049858/83356707-1441bc00-a368-11ea-9ce3-ab17fb81a74b.jpg)

![PiMKRHAT with Raspberry Pi](https://user-images.githubusercontent.com/3049858/83356709-16a41600-a368-11ea-9101-fdaf97b5e9ee.jpg)

![PiMKRHAT and stacked MKR Shields](https://user-images.githubusercontent.com/3049858/83356701-0e4bdb00-a368-11ea-8c06-ff7c251af9ee.jpg)

# Installation for MKR ENV

![Arduino MKR ENV Shield](https://user-images.githubusercontent.com/3049858/79135621-eef4f080-7daf-11ea-97a6-8760266a50bb.jpg)

1. Download the [latest release](https://drive.google.com/open?id=1mo6LHWPsm_JBmMwiMcn8H-1lESI1KIQK)
2. Unzip the downloaded file
3. Write the image to your SD card. See [here](https://www.raspberrypi.org/documentation/installation/installing-images/README.md) for details.
4. Boot your Raspberry Pi and wait for WeatherPi_TFT to start.

# Configuration

##  Wifi settings
You can follow this [tutorial](https://www.raspberrypi.org/documentation/configuration/wireless/headless.md) to setting the Wifi headless. 

or you can use a Raspberry Pi (2/3/4) connected to Ethernet via Putty and SSH:
```bash
sudo raspi-config
--> 2 Network Options
--> N2 Wi-fi
``` 

## Localisation
```bash
sudo raspi-config
--> 4 Localisation Options
--> I1 Change Locale 
--> change your language ISO-8859-1 locales
``` 
Please note you can choose under 4 Localisation Options your time zones too!

## Edit config file
```bash
cd
cd WeatherPi_TFT
sudo nano config.json
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


# License

This library is free software; you can redistribute it and/or
modify it under the terms of the GNU Lesser General Public
License as published by the Free Software Foundation; either
version 2.1 of the License, or (at your option) any later version.

This library is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
Lesser General Public License for more details.


