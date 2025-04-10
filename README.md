 

<p align=center>
  <a href="https://www.instagram.com/hackethics138/"><img title="Made in INDIA" src="https://img.shields.io/badge/MADE%20IN-INDIA-SCRIPT?colorA=%23ff8100&colorB=%23017e40&colorC=%23ff0000&style=for-the-badge"></a>
  </p>

###### <p align="center"> *locationTracker*

  <br>

<p align="center"><img src="https://github.com/H4ckethics138/locationTracker/blob/main/res/Screenshot_2025_0407_161530.jpg"></p>

###### <p align="center">Accurate GPS Location Tracker (Android, IOS, Windows phones.)
<p align=center>
  <a href="https://www.instagram.com/hackethics138/"><img title="Open Source" src="https://img.shields.io/badge/Open%20Source-%E2%99%A5-red" ></a>
  <a href="https://www.instagram.com/hackethics138/"><img title="GitHub version" src="https://d25lcipzij17d.cloudfront.net/badge.svg?id=gh&type=6&v=1.0&x2=0" ></a>
  <a href="https://www.instagram.com/hackethics138/"><img title="Stars" src="https://img.shields.io/github/stars/bhikandeshmukh/MapEye?style=social" ></a>
  <a href="https://github.com/H4ckethics138/followers"><img title="Followers" src="https://img.shields.io/github/followers/bhikandeshmukh?color=blue&style=flat-square"></a>

  <a href="#"><img src="https://badges.pufler.dev/visits/bhikandeshmukh/MapEye">

###### <p align="center">*This is official repository maintained by us*
###### <p align="center"> *[**vikash jangid**](https://www.instagram.com/hackethics138//) ❤️*
###### <p align="center"> *You can check [Instagram](https://www.instagram.com/hackethics138/)✌*

## locationTracker 

Concept behind main.py is simple, just like we host phishing pages to get credentials why not host a fake page that requests your location like many popular location based websites. Read more on vikash jangid's Blog main.py Hosts a fake website which asks for Location Permission and if the target allows it, we can get :

* Longitude
* Latitude
* Accuracy
* Altitude - Not always available
* Direction - Only available if user is moving
* Speed - Only available if user is moving

Along with Location Information we also get **Device Information** without any permissions :

* Unique ID using Canvas Fingerprinting
* Device Model - Not always available
* Operating System
* Platform
* Number of CPU Cores - Approximate Results
* Amount of RAM - Approximate Results
* Screen Resolution
* GPU information
* Browser Name and Version
* Public IP Address
* Local IP Address
* Local Port

**Automatic IP Address Reconnaissance** is performed after the above information is received.

**This tool is a Proof of Concept and is for Educational Purposes Only, mapeye.py shows what data a malicious website can gather about you and your devices and why you should not click on random links and allow critical permissions such as Location etc.**

## How is this Different from IP GeoLocation

* Other tools and services offer IP Geolocation which is NOT accurate at all and does not give location of the target instead it is the approximate location of the ISP.

* main.py uses HTML API and gets Location Permission and then grabs Longitude and Latitude using GPS Hardware which is present in the device, so mapeye.py works best with Smartphones, if the GPS Hardware is not present, such as on a Laptop, mapeye.py fallbacks to IP Geolocation or it will look for Cached Coordinates.  

* Generally if a user accepts location permsission, Accuracy of the information recieved is **accurate to approximately 30 meters**

* Accuracy depends on multiple factors which you may or may not control such as :
  * Device - Won't work on laptops or phones which have broken GPS
  * Browser - Some browsers block javascripts
  * GPS Calibration - If GPS is not calibrated you may get inaccurate results and this is very common

## Templates

Available Templates :

* NearYou
* Google Drive
* WhatsApp group
* Telegram

## Tested On :

* Kali Linux
* BlackArch Linux
* Ubuntu
* Kali Nethunter
* Termux
* Parrot OS

## Installation

### Basic For Beginners

```bash
git clone https://github.com/H4ckethics138/locationTracker.git
cd locationTracker
python3 main.py -t manual -k testkml
```
Choose Options Batween 0 to 3

### you can use packetriot

### ngrok setup

```bash
go to ngrok.com (Login)
Download ngrok
$ unzip ngrok.zip
$ ./ngrok authtoken *******
$ ./ngrok http 8080
send link to victim
```

### Kali Linux / Ubuntu / Parrot OS

```bash
git clone https://github.com/H4ckethics138/locationTracker.git
cd locationTracker
apt update
apt install python3 python3-pip php
pip3 install requests
python3 main.py
```

### BlackArch Linux

```bash
pacman -S mian.py
```

### Termux

```bash

cd locationTracker
pkg update
pkg install python php
pip3 install requests
```

## Usage

```bash
python3 main.py -h

usage: main.py [-h] [-s SUBDOMAIN]

optional arguments:
  -h, --help            show this help message and exit
  -k KML, --kml         Provide KML Filename ( Optional )
  -p PORT, --port       Port for Web Server [ Default : 8080 ]
  -t TUNNEL, --tunnel   Specify Tunnel Mode [ Available : manual ]

##################
# Usage Examples #
##################

# Step 1 : In first terminal
$ python3 main.py -t manual

# Step 2 : In second terminal start a tunnel service such as ngrok
$ ./ngrok http 4545

###########
# Options #
###########

# Ouput KML File for Google Earth
$ python3 main.py -t manual -k <filename>

# Use Custom Port
$ python3 mapin.py -t manual -p 1337
$ ./ngrok http 1337

```

### Legal Disclaimer :

Usage of the tool for attacking targets without prior mutual consent is illegal. It's the end user's responsibility to obey all applicable local, state and federal laws. Developers assume no liability and are not responsible for any misuse or damage caused by this program

-------------------------------------------------------------------------------------

### Development by

Developer / Author: [vikash jangid ](https://www.instagram.com/hackethics138/)

###### <p align="center">To Know about Ethical Hacking , Android And Kali Linux Do ♨️ Follow ♨️ Us:-</p>
<p align="center">
<a href="https://www.instagram.com/hackethics138//"><img title="Instagram" src="https://img.shields.io/badge/instagram-%23E4405F.svg?&style=for-the-badge&logo=instagram&logoColor=white"></a>
<a href="https://wa.me/919571978339"><img title="whatsapp" src="https://img.shields.io/badge/WHATSAPP-%2325D366.svg?&style=for-the-badge&logo=whatsapp&logoColor=white"></a>
<a href="https://t.me/hackethics138_pvtChannel_bot"><img title="Telegram" src="https://img.shields.io/badge/Telegram-blue?style=for-the-badge&logo=Telegram"></a>

-------------------------------------------------------------------------------------
