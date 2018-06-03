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

```
