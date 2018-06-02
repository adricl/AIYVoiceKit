# AIYVoiceKit

## How to setup AIY Voice Kit on a PI from scratch  

Flash a headless version of raspbian

Sudo apt update

Sudo apt upgrade

Sudo raspi-config 

sudo rpi-update

Expand disk 

Enable ssh

git clone -b voicekit https://github.com/google/aiyprojects-raspbian.git
cd ~/voice-recognizer-raspi

FOr this part you can also read https://github.com/google/aiyprojects-raspbian/blob/master/HACKING.md#installing-the-voice-hat-driver-and-config

sudo ./scripts/install-deps.sh

sudo scripts/install-services.sh

sudo apt-get update
sudo apt-get install raspberrypi-kernel
sudo scripts/configure-driver.sh
sudo scripts/install-alsa-config.sh
sudo reboot


Sudo pip3 install google-cloud
sudo pip3 install google-assistant-sdk
sudo pip3 install google-assistant-grpc
sudo pip3 install google-assistant-library

