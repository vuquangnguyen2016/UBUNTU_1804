# UBUNTU_1804
# cai dat unikey
```
sudo apt-get update
sudo apt-get install ibus-unikey	
ibus restart

im-config
ibus-setup
```

# CAI DAT LATEX
```
sudo add-apt-repository ppa:jonathonf/texlive-2017
sudo apt-get update
sudo apt-get install texlive-full
```
## CAI DAT OBS
```
 sudo apt-get install ffmpeg
  sudo add-apt-repository ppa:obsproject/obs-studio
   sudo apt-get update && sudo apt-get install obs-studio

```

## CAI DAT NVIDIA
```
 sudo add-apt-repository ppa:graphics-drivers
  sudo apt-get update 
  
  sudo apt-get remove --purge nvidia-*
sudo apt-get purge nvidia* bumblebee primus bbswitch-dkms

sudo mv /etc/X11/xorg.conf /etc/X11/xorg.conf.backup

sudo add-apt-repository ppa:graphics-drivers/ppa
sudo apt update
sudo apt upgrade
sudo apt install nvidia-driver-396

 ```
## CAI DAT R
```
