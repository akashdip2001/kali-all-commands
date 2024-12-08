<img align="right" alt="Mechanical Engineering" width="400" src="https://user-images.githubusercontent.com/81384987/206849634-955fcda0-a46b-4624-a5ad-fa4ffa1eef43.png"> 

# kali-all-commands

<br>

- 🔭 I’m currently working on [**my web-site**](https://akashdip2001.github.io/linktree/)

<br>
<br>
<a href="https://www.youtube.com/c/akash aot" target="blank"><img align="center" src="https://user-images.githubusercontent.com/81384987/209952974-0163b04e-ccae-4be5-844a-075ef85c43d2.png" alt="akash aot" height="30" width="40" />  My YouTube Channel</a>
<br>
<br>

---
---
# Add Kali Repositirie
<h3> jast copy & past the code into your Terminal - Done ✔️  </h3>

```
echo "deb http://http.kali.org/kali kali-rolling main contrib non-free" | sudo tee /etc/apt/sources.list
```

[`offical Website`](https://www.kali.org/docs/general-use/kali-linux-sources-list-repositories/)

---
# No sound on Kali
```
sudo apt purge --autoremove pipewire-pulse
```
[`offical Website`](https://www.kali.org/docs/troubleshooting/no-sound/)

---
# Any previous installation not successfully completed
```
apt --fix-broken install
```

---

# WIFI Connect but Not working 
```
sudo systemctl status systemd-resolved.service 
sudo systemctl restart systemd-resolved.service (only this )
sudo systemctl status systemd-resolved.service 
```
---
# Turn ON Bluetooth
```
service bluetooth restart
```
---
# Install Softwers in KALI Linux ---
```
sudo dpkg -i *.deb                ( normal .deb file install command )
./configure  ---  make install    ( install Python in Kali command )
```       
       
[**How to install all type of softwers in KALI linux**](https://youtu.be/fDod27oOZCM)      

---
<h3>Snap Install</h3>

```
sudo su
sudo apt update
sudo apt install snapd
apt update
apt install snapd
systemctl enable --now snapd apparmor
```

Snap install but not Working ---
```
systemctl enable --now snapd.apparmor
```         
[**How to install Snap Store in KALI linux**](https://youtu.be/P_qg4ujwypE)

---

# Uninstall  --- 
```
dpkg --list
sudo apt remove gimp
sudo apt --purge remove gimp
sudo apt-get autoremove
sudo apt purge --auto-remove gimp
sudo apt clean
```
---
# force STOP any running Program
```
pidof [appname]
kill -9 [number]
```
---
# All imp. Softwers in KALI and all [Tools](https://www.kali.org/tools/all-tools/)

| Name  |    Work       |  normal Code  | snap Code | flathub Code |
|-----|-------------|---------------|---------------|---------------|
|~~~~~~~~~~~~~~~~~~~~|~~~~~~~~~~~~~~~~ |~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ |~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ |~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ |
| | |FIRST_ADD_KALI_REPOSITORY [`link`](https://www.kali.org/docs/general-use/kali-linux-sources-list-repositories/) | FIRST_ISTALL_SNAP_THEN_USE_IT [`link`](https://snapcraft.io/docs/installing-snapd) | FIRST_SETUP_FLATHUB [`link`](https://flatpak.org/setup/) |
|~~~~~~~~~~~~~~~~~~~~|~~~~~~~~~~~~~~~~ |~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ |~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ |~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ |
| office 360 | Microsoft [`link`](https://snapcraft.io/office365webdesktop) | |sudo snap install office365webdesktop --beta
| wats app | Messaging app | |sudo snap install whatsapp-for-linux |flatpak install flathub com.github.eneshecan.WhatsAppForLinux
| telegram | Messaging_app | |sudo snap install telegram-desktop|flatpak install flathub org.telegram.desktop
| viber | Messaging app | app Downlod [`link`](https://www.viber.com/en/download/) |sudo snap install viber-unofficial |flatpak install flathub com.viber.Viber
| google message | Messaging app | scan the code using phon [`link`](https://messages.google.com/web)
| kdeconnect | File transfer | sudo apt install kdeconnect
| freecad | Engineering_Drawing |sudo apt install freecad|sudo snap install freecad|flatpak install flathub org.freecadweb.FreeCAD
| shotcut | Video Editor |sudo apt install shotcut|sudo snap install shotcut --classic|[`link`](https://flathub.org/apps/details/org.shotcut.Shotcut)
| gimp | Photo Editor |
| simplescreenrecorder | Screen recorder |sudo apt install simplescreenrecorder
| audacity | Audio Editor |
| handbrake | Video compressor |
| codeblocks | Coding |
| blender | Graphic design |
| freeDownloadManager |
| ktouch | Typing Pracktice |
| virtualbox |
| terminator |
| edge | Browser
| audacious | mp3 player |

---

# Delet File --  
```
rm [file location]   (for Empty file)
rm -r [...]          (for a directory)
```
---
# install Wine -- (Windows emulator for linux)
```
sudo dpkg --add-architecture i386
sudo apt update
sudo apt install wine wine64 wine32 winbind winetricks
wine xxxxxx.exe
```
<img src="https://github.com/akashdip2001/college-final-year-project/raw/main/img/colour_line.png">

[<img align="right" alt="Mechanical Engineering" width="400" src="img/wsl.jpg">](https://youtu.be/JQDbcyRa5_0)

## WAL 2 [Video](https://youtube.com/playlist?list=PL_RecMEcs_p-iAMEQascgKVMt4juhGip2&si=nzpb4GEv-QxkROI6)
### Kali in Windows

```go
// Windows PowerShell
// Copyright (C) Microsoft Corporation. All rights reserved.
// PS C:\WINDOWS\system32> wsl --status

wsl --install
wsl --update
wsl --status
wsl --list --online
wsl --install -d kali-linux

// set userName : XXXX
// set Passward : 1XX
```
<img src="img/wsl remote desktop connect (3).png">

### in Kali cell
```
cat /etc/os-release
// PRETTY_NAME="Kali GNU/Linux Rolling"
// NAME="Kali GNU/Linux"
// VERSION_ID="2024.3"
// VERSION="2024.3"
// VERSION_CODENAME=kali-rolling
// ID=kali
// ID_LIKE=debian
// HOME_URL="https://www.kali.org/"
// SUPPORT_URL="https://forums.kali.org/"
// BUG_REPORT_URL="https://bugs.kali.org/"
// ANSI_COLOR="1;31"
```
## Install `mini` Desktop envirorment with `kex server` (❌ not Recommended ❌)
```
sudo apt update && sudo apt upgrade -y
sudo apt install kali-win-kex
kex --win -s
// set passward (6) Ex: 1XXAs0
// then enter Kali pass : 1XX

kex --esm --ip -s // for Wondows Remote Desktop
```
<img src="img/wsl remote desktop connect (1).png">
<img src="img/wsl remote desktop connect.png">

### Shut Down
```
exit
wsl --shutdown
```
### Uninstall kex
```
// Uninstall Win-KeX and Xfce
sudo apt purge kali-win-kex
sudo apt purge xfce4 xfce4-goodies
sudo apt autoremove --purge

// Uninstall the Current Desktop Environment (Xfce and Win-KeX)
sudo apt purge kali-win-kex xfce4 xfce4-goodies
sudo apt purge lightdm light-locker
sudo apt autoremove --purge
sudo apt clean
```
## Install `Full` Desktop envirorment (✅ Recommended ✅)
```
// Install the GNOME Desktop Environment
sudo apt update
sudo apt install kali-desktop-gnome gdm3

// Set GNOME as the Default Environment
sudo update-alternatives --config x-session-manager

// Restart WSL or the System
wsl --shutdown
wsl

// To be continue ... 
```
---

| <a href="https://akashdip2001.github.io/ubuntu-all-commaands/" class="previous">&laquo; Ubuntu linux all commands</a> <br/> |
|-----------------------------------------------------------------------------------------------------------------------------|
| <a href="https://akashdip2001.github.io/fedora-all-imp-commands/" class="next">Fedora linux all commands &raquo;</a> |

---
✔️ [**my Website**](https://akashdip2001.github.io/linktree/)
<h1 align="right">AKASHDIP MAHAPATRA</h1>
<h3 align="right">National award from Dilhi,taken from Indian precedent Pronob Mukherjee 2012,Drawing</h3>
<h5 align="right">https://youtu.be/ysBF9EfvWkk?t=428</h5>

---

<h3 align="left">Connect with me:</h3>
<p align="left">


<a href="https://linkedin.com/in/akashdip-mahapatra-330687204" target="blank"><img align="center" src="https://user-images.githubusercontent.com/81384987/209952833-314ab313-7120-4755-b65c-b573098387b3.png" alt="akashdip-mahapatra-330687204" height="40" width="40" /></a>
<a href="https://www.youtube.com/c/akash aot" target="blank"><img align="center" src="https://user-images.githubusercontent.com/81384987/209952974-0163b04e-ccae-4be5-844a-075ef85c43d2.png" alt="akash aot" height="35" width="50" /></a>
<a href="https://akashdip2001.github.io/linktree/" target="blank"><img align="center" src="https://yt3.ggpht.com/7tPHyFi7-QyTnhpc484ZzTuRp0fZSY-CUuykvzuKdKYIwt0fmw98SWMqwRy_7pZ6LQzEYJlvXA=s88-c-k-c0x00ffffff-no-rj-mo" alt="akashdip2001" height="40" width="40" /></a>

</p>
