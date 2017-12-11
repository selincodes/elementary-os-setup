# My setup after installation Elementary OS loki

#### 1. Update system
```
sudo apt update && sudo apt upgrade
```

#### 2. Enable PPA
```
sudo apt install software-properties-common
sudo apt install software-properties-gtk
sudo software-properties-gtk
```

#### 3. Install elementary Tweaks
```
sudo add-apt-repository ppa:philip.scott/elementary-tweaks
sudo apt update
sudo apt install elementary-tweaks
```
![alt text](https://pp.userapi.com/c840732/v840732340/2d76c/xFY6lL-y0N0.jpg "Elementary Tweaks")

#### 4. Install TLP to save battery and prevent overheating
```
sudo apt install tlp tlp-rdw
sudo tlp start
```

#### 5. Install Firefox
```
sudo apt install firefox
```

#### 6. Install Chromium
```
sudo apt install -y chromium-browser
````
> If you need Flash, run the following command

```
sudo apt install -y pepperflashplugin-nonfree
sudo update-pepperflashplugin-nonfree --install
```

#### 7. Install VLC
```
sudo apt install vlc
```

#### 8. Install Filezilla
```
sudo apt install filezilla
```

#### 9. Install Ubuntu Restricted extras
> mp3, avi, mpeg, TrueType, Java, Flash, Codecs
```
sudo apt install ubuntu-restricted-extras
```

#### 10. Install Gimp
```
sudo apt install gimp
```

#### 11. Install inkscape
```
sudo apt install inkscape
```

#### 12. Install Sublime Text
> 3154 change to version number
```
wget https://download.sublimetext.com/sublime-text_build-3154_amd64.deb
cd ~/Downloads
sudo dpkg -i sublime-text_build-3154_amd64.deb
```
> License for 3154
```
----- BEGIN LICENSE -----
eldon
Single User License
EA7E-1122628
C0360740 20724B8A 30420C09 6D7E046F
3F5D5FBB 17EF95DA 2BA7BB27 CCB14947
27A316BE 8BCF4BC0 252FB8FF FD97DF71
B11A1DA9 F7119CA0 31984BB9 7D71700C
2C728BF8 B952E5F5 B941FF64 6D7979DA
B8EB32F8 8D415F8E F16FE657 A35381CC
290E2905 96E81236 63D2B06D E5F01A69
84174B79 7C467714 641A9013 94CA7162
------ END LICENSE ------
```

#### 13. Install Eddy
> A debian package installer for elementary OS


[![Get it on AppCenter](https://appcenter.elementary.io/badge.svg)](https://appcenter.elementary.io/com.github.donadigo.eddy)
![alt text](https://pp.userapi.com/c840732/v840732112/2c401/p0OyT-G4aiQ.jpg "Eddy")

#### 14. Install Node.js
```
curl -sL https://deb.nodesource.com/setup_8.x | sudo -E bash -
sudo apt update
sudo apt install -y nodejs
nodejs -v && npm -v
```

#### 15. Install Git, Gulp
```
sudo apt install git
sudo npm install --global gulp
```

#### 16. Install qbittorrent
```
sudo apt install qbittorrent
```

#### 17. Install MS Fonts
```
sudo apt install ttf-mscorefonts-installer
cd /tmp && wget http://www.stchman.com/tools/MS_fonts/tahoma.zip
sudo unzip -d /usr/share/fonts/truetype/msttcorefonts /tmp/tahoma.zip
fc-cache -fv
```

#### 18. Install Viber and Telegram
```
http://download.cdn.viber.com/cdn/desktop/Linux/viber.deb

sudo add-apt-repository ppa:atareao/telegram
sudo apt update
sudo apt install telegram
```

#### 19. Install Avocode
> More info https://help.avocode.com/app-settings/installing-avocode-on-linux
```
echo deb http://linux.avocode.com/apt all main >> /etc/apt/sources.list
sudo apt update
sudo apt install avocode
```

#### 20. Install Photoshop
> Download and install CrossOver
```
http://nnm-club.name/forum/viewtopic.php?t=1150815
```
> Download Photoshop
```
http://nnm-club.name/forum/viewtopic.php?t=1139590
```
> Restore with CrossOver
```
Bottle -> Import bottle archive
```






#### Remove PPA
```
sudo add-apt-repository --remove ppa:whatever/ppa
```
#### Remove apps
```
sudo apt purge _name_
sudo apt remove _name_
sudo apt autoremove && sudo apt autoclean
```























