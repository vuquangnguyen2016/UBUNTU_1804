# Activate MS OFFICE 2016

```


https://www.tranbadat.com/2017/10/huong-dan-nhan-ban-quyen-office-2016.html


cd C:\Program Files\Microsoft Office\Office16
cscript OSPP.VBS /inpkey:XQNVK-8JYDB-WJ9W3-YJ8YR-WFG99
cscript OSPP.VBS /sethst:kms.digiboy.ir
cscript OSPP.VBS /act
cscript OSPP.VBS /dstatus

Office Professional Plus 2016: XQNVK-8JYDB-WJ9W3-YJ8YR-WFG99
Office Standard 2016 : JNRGM-WHDWX-FJJG3-K47QV-DRTFM
Project Professional 2016: YG9NW-3K39V-2T3HJ-93F3Q-G83KT
Project Standard 2016: GNFHQ-F6YQM-KQDGJ-327XX-KQBVC
Visio Professional 2016: PD3PC-RHNGV-FXJ29-8JK7D-RJRJK
Visio Standard 2016: 7WHWN-4T7MP-G96JF-G33KR-W8GF4
Access 2016: GNH9Y-D2J4T-FJHGG-QRVH7-QPFDW
Excel 2016: 9C2PK-NWTVB-JMPW8-BFT28-7FTBF
OneNote 2016: DR92N-9HTF2-97XKM-XW2WJ-XW3J6
Outlook 2016: R69KK-NTPKF-7M3Q4-QYBHW-6MT9B
PowerPoint 2016: J7MQP-HNJ4Y-WJ7YM-PFYGF-BY6C6
Publisher 2016: F47MM-N3XJP-TQXJ9-BP99D-8K837
Skype for Business 2016: 869NQ-FJ69K-466HW-QYCP2-DDBV6
Word 2016: WXY84-JN2Q9-RBCCQ-3Q3J3-3PFJ6

```



# Active windows 10

```

https://drive.google.com/file/d/11G2aC7gX1pyktm_PygDOLrVhZ9cKsato/view


```



# UBUNTU_1804

### Creating a Windows 10 Bootable USB for UEFI Firmware
```
https://www.linuxbabe.com/ubuntu/easily-create-windows-10-bootable-usb-ubuntu

sudo apt install gparted

```

```

# Increase Battery Life of Linux Laptops using PowerTop  
sudo apt-get install powertop
sudo powertop
sudo powertop --auto-tune

# powersave
power-save
sudo pm-powersave true

#-------------
sudo apt-get install cpufrequtils
sudo nano /etc/default/cpufrequtils


Install cpufrequtils:

$ sudo apt-get install cpufrequtils

Then edit the following file (if it doesn't exist, create it):

$ sudo nano /etc/default/cpufrequtils

And add the following line to it:

  GOVERNOR="performance"

Save and exit.

To changes take effect, run:

$ sudo /etc/init.d/cpufrequtils restart

Then you can run cpufreq-info to see informations about your cpu frequency, governor and more:

$ cpufreq-info
    current policy: frequency should be within 800 MHz and 3.90 GHz.
              The governor "performance" may decide which speed to use
              within this range.

```


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

sudo apt-get update
sudo apt-get install gdebi libxml2-dev libssl-dev libcurl4-openssl-dev libopenblas-dev r-base r-base-dev

# Install R
sudo apt-get update
sudo apt-get install gdebi libxml2-dev libssl-dev libcurl4-openssl-dev libopenblas-dev r-base r-base-dev

# Install RStudio
cd ~/Downloads
wget https://download1.rstudio.org/rstudio-xenial-1.1.383-amd64.deb
sudo gdebi rstudio-xenial-1.1.383-amd64.deb
printf '\nexport QT_STYLE_OVERRIDE=gtk\n' | sudo tee -a ~/.profile



# install common packages
R --vanilla << EOF
install.packages(c("tidyverse","data.table","dtplyr","devtools","roxygen2","bit64"), repos = "https://cran.rstudio.com/")
q()
EOF

# Export to HTML/Excel
R --vanilla << EOF
install.packages(c("htmlTable","openxlsx"), repos = "https://cran.rstudio.com/")
q()
EOF

# Blog tools
R --vanilla << EOF
install.packages(c("knitr","rmarkdown"), repos='http://cran.us.r-project.org')
q()
EOF
sudo apt-get install python-pip
sudo pip install markdown rpy2==2.7.8 pelican==3.6.3

# PDF extraction tools
sudo apt-get install libpoppler-cpp-dev default-jre default-jdk r-cran-rjava
sudo R CMD javareconf
R --vanilla << EOF
library(devtools)
install.packages("pdftools", repos = "https://cran.rstudio.com/")
install_github("ropensci/tabulizer")
q()
EOF

# TTF/OTF fonts usage
sudo apt-get install libfreetype6-dev
R --vanilla << EOF
install.packages("showtext", repos = "https://cran.rstudio.com/")
q()
EOF

# Cairo for graphic devices
sudo apt-get install libgtk2.0-dev libxt-dev libcairo2-dev
R --vanilla << EOF
install.packages("Cairo", repos = "https://cran.rstudio.com/")
q()
EOF

```

## CAI THEME
```
sudo apt-get install gnome-tweak-tool
https://www.youtube.com/watch?v=sfsKwzElxQg
sudo apt-get install chrome-gnome-shell

.themes
.icons
dash to dock



```
## RAM 
```
1. Connect ssh to your Ec2 Instance.

2. Become the super user after executing the command sudo -s 

3. Check the amount of used and free memory in the system in real time using the following command watch -n 3 free -m 

4. To get the detailed real time information about memory usage, use the following command watch -n 3 cat /proc/meminfo 

5. Execute the following command to release the Page Cache echo 1 &lt; /proc/sys/vm/drop_caches 



6. Execute the following command to release the Dentries and Inodes echo 2 &lt; /proc/sys/vm/drop_caches 

7. Now execute the following command to release the Dentries and Inodes and Page Cache echo 3 &lt; /proc/sys/vm/drop_caches 

8. Now check again amount of usded and released memory watch -n 3 free -m 

9. Flush the File System Buffers using the following command sync
```

