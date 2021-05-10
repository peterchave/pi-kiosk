# pi-kiosk

Sets up a Raspberry Pi in a simple kiosk mode

## Raspberry Pi setup

Setup Pi in basic chrome kiosk mode, instructions adapted from: https://die-antwort.eu/techblog/2017-12-setup-raspberry-pi-for-kiosk-mode/

### Step by step

* Download Raspberry Pi OS (32-bit) Lite from https://www.raspberrypi.org/downloads/raspberry-pi-os/
* Use etcher https://www.balena.io/etcher/ (or similar) to burn onto a 2Gb (or larger) microSD
* Boot up Pi
* Initial config (`sudo raspi-config`)
  * Change user password 
  * Setup networking
  * Boot options = "Desktop/CLI" → "Console Autologin"
  * Interfacing options: "Enable SSH"
* Run install script:
  * `bash <(curl -sL https://raw.githubusercontent.com/peterchave/pi-kiosk/main/install)`
