# General

##Intel HD 4000 1440x2560

https://www.notebookcheck.net/2560x1440-or-2560x1600-via-HDMI.92840.0.html

cvt 2560 1440 30

###Best option:
xrandr --newmode "2560x1440" 220.812 2560 2608 2640 2720 1440 1443 1448 1478 -hsync -vsync
xrandr --addmode HDMI2 "2560x1440"

###To know output: 
xrandr

###Save Here to Autostart:
sudo nano /etc/X11/xorg.conf


## FIREFOX YOUTUBE 
We need to setting these keys to true in about:config, it's a must for firefox users who watch youtube. Restart firefox after. layers.acceleration.force-enabled 
webgl.force-enabled 
media.hardware-video-decoding.force-enabled 

## Arch Package Manager Error
sudo pacman-mirrors -f
sudo pacman -Syyu

## ARDUINO
sudo chmod a+rw /dev/ttyACM0

## ARCH CLEAR CACHE
sudo pacman -Rsn $(pacman -Qdtq)
sudo pacman -Scc
sudo rm /var/lib/systemd/coredump/. ---NAO TRABALHA
sudo journalctl --vacuum-size=50M

## MySQL
https://medium.com/@shivraj.jadhav82/mysql-setup-on-linux-mint-948470115d5
sudo apt-get remove --purge mysql*  
sudo apt-get purge mysql*  
sudo apt-get autoremove  
sudo apt-get autoclean  
sudo apt-get remove dbconfig-mysql





