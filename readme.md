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

#### 3. Install TP-Link driver
```
sudo apt install git dkms
git clone https://github.com/jeremyb31/rtl8812au-1.git
cd rtl8812au-1
sudo ./dkms-install.sh
```

#### 4. Install elementary Tweaks
```
sudo add-apt-repository ppa:philip.scott/elementary-tweaks
sudo apt update
sudo apt install elementary-tweaks
```
![alt text](https://pp.userapi.com/c840732/v840732340/2d76c/xFY6lL-y0N0.jpg "Elementary Tweaks")

#### 5. Install TLP to save battery and prevent overheating
```
sudo apt install tlp tlp-rdw
sudo tlp start
```

#### 6. Install Firefox
```
sudo apt install firefox
```

#### 7. Install Chromium
```
sudo apt install -y chromium-browser
````
> If you need Flash, run the following command

```
sudo apt install -y pepperflashplugin-nonfree
sudo update-pepperflashplugin-nonfree --install
```

#### 8. Install VLC
```
sudo apt install vlc
```

#### 9. Install Filezilla
```
sudo apt install filezilla
```

#### 10. Install Ubuntu Restricted extras
> mp3, avi, mpeg, TrueType, Java, Flash, Codecs
```
sudo apt install ubuntu-restricted-extras
```

#### 11. Install Gimp
```
sudo apt install gimp
```

#### 12. Install inkscape
```
sudo apt install inkscape
```

#### 13. Install Sublime Text
> 3207 change to version number
```
cd ~/Downloads
wget https://download.sublimetext.com/sublime-text_build-3207_amd64.deb
sudo dpkg -i sublime-text_build-3207_amd64.deb
```
> Added these lines into sudo gedit /etc/hosts
```
127.0.0.1       www.sublimetext.com
127.0.0.1       license.sublimehq.com
```
> License for 3207
```
----- BEGIN LICENSE -----
Member J2TeaM
Single User License
EA7E-1011316
D7DA350E 1B8B0760 972F8B60 F3E64036
B9B4E234 F356F38F 0AD1E3B7 0E9C5FAD
FA0A2ABE 25F65BD8 D51458E5 3923CE80
87428428 79079A01 AA69F319 A1AF29A4
A684C2DC 0B1583D4 19CBD290 217618CD
5653E0A0 BACE3948 BB2EE45E 422D2C87
DD9AF44B 99C49590 D2DBDEE1 75860FD2
8C8BB2AD B2ECE5A4 EFC08AF2 25A9B864
------ END LICENSE ------
```
> Sublime text 3 packages
```
A File Icon
AutoFileName
Dracula Color Scheme
Emmet
Sass
SideBarEnhancements
M3U
Djaneiro
requirementstxt
SublimeLinter
GitGutter
```
> Sublime text 3 settings
```
{
	"update_check": false,
	"auto_complete": false,
	"color_scheme": "Packages/Dracula Color Scheme/Dracula.tmTheme",
	"font_face": "Roboto Mono Medium",
	"font_size": 11,
	"highlight_line": true,
	"ignored_packages":
	[
		"Vintage"
	],
	"menu_visible": true,
	"theme": "Adaptive.sublime-theme",
	"word_wrap": true
}
```

#### 14. Install Eddy
> A debian package installer for elementary OS


[![Get it on AppCenter](https://appcenter.elementary.io/badge.svg)](https://appcenter.elementary.io/com.github.donadigo.eddy)
![alt text](https://pp.userapi.com/c840732/v840732112/2c401/p0OyT-G4aiQ.jpg "Eddy")

#### 15. Install Node.js
```
curl -sL https://deb.nodesource.com/setup_8.x | sudo -E bash -
sudo apt update
sudo apt install -y nodejs
nodejs -v && npm -v
```

#### 16. Install Git, Gulp
```
sudo apt install git
sudo npm install --global gulp
```

#### 17. Install qbittorrent
```
sudo apt install qbittorrent
```

#### 18. Install MS Fonts
```
sudo apt install ttf-mscorefonts-installer
cd /tmp && wget http://www.stchman.com/tools/MS_fonts/tahoma.zip
sudo unzip -d /usr/share/fonts/truetype/msttcorefonts /tmp/tahoma.zip
fc-cache -fv
```

#### 19. Install Viber and Telegram
```
http://download.cdn.viber.com/cdn/desktop/Linux/viber.deb

sudo add-apt-repository ppa:atareao/telegram
sudo apt update
sudo apt install telegram
```

#### 20. Install Avocode
> More info https://help.avocode.com/app-settings/installing-avocode-on-linux
```
echo deb http://linux.avocode.com/apt all main >> /etc/apt/sources.list
sudo apt update
sudo apt install avocode
```

#### 21. Install Photoshop
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

#### 22. Install Atom
```
sudo add-apt-repository ppa:webupd8team/atom
sudo apt update && sudo apt install atom
```





#### Remove PPA
```
sudo add-apt-repository --remove ppa:whatever/ppa
```
#### Remove apps
```
sudo apt remove --purge _name_
sudo apt autoremove && sudo apt autoclean
```























