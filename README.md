<img align="right" alt="Mechanical Engineering" width="400" src="https://user-images.githubusercontent.com/81384987/206849634-955fcda0-a46b-4624-a5ad-fa4ffa1eef43.png"> 

# kali-all-commands
[![YouTube](https://yt3.ggpht.com/7tPHyFi7-QyTnhpc484ZzTuRp0fZSY-CUuykvzuKdKYIwt0fmw98SWMqwRy_7pZ6LQzEYJlvXA=s88-c-k-c0x00ffffff-no-rj-mo)](https://www.youtube.com/channel/UCxvmp634YDc41xCWOdvWqoQ)
<br>
- 🔭 I’m currently working on [**my web-site**](https://akashdip2001.github.io/linktree/)


<h6 align="right">all imp. commands of KALI LINUX. This repositry helps to install, Uninstall, WIFI peoblams, all usefull apps </h6>
<br>
<br>

---
# Add Kali Repositirie ( jast copy & past the code into your Terminal - Done ✔️  )
```
echo "deb http://http.kali.org/kali kali-rolling main contrib non-free" | sudo tee /etc/apt/sources.list
```

| [**offical Website**](https://www.kali.org/docs/general-use/kali-linux-sources-list-repositories/) |
|---|

---
# No sound on Kali
```
sudo apt purge --autoremove pipewire-pulse
```

| [**offical Website**](https://www.kali.org/docs/troubleshooting/no-sound/) |
|---|

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
# All imp. Softwers in KALI

| Name                      |   Work    |  Code   |
|----------------------------|:-----------:|:------------:|
| wats app | messaging app | sudo snap install whatsapp-for-linux |
| telegram | messaging app | sudo snap install telegram-desktop |
| viber | messaging app | Downlod [`link`](https://www.viber.com/en/download/) |
| google message | messaging app |
| kdeconnect | file transfer | sudo apt install [name]
| freecad | Engineering Drawing |
| shotcut | Video Editor |
| gimp | photo Editor |
| simplescreenrecorder | screen recorder |
| audacity | audio Editor |
| handbrake | video compressor |
| codeblocks | coding |
| blender | graphic design |
| freeDownloadManager |
| ktouch | Typing Pracktice |
| virtualbox |
| terminator |
| edge | 
| audacious | mp3 player |


# Delet File --  
```
rm [file location]   (for Empty file)
rm -r [...]          (for a directory)
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

<h3 align="left">Connect with me:</h3>
<p align="left">


<a href="https://linkedin.com/in/akashdip-mahapatra-330687204" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/linked-in-alt.svg" alt="akashdip-mahapatra-330687204" height="30" width="40" /></a>
<a href="https://www.youtube.com/c/akash aot" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/youtube.svg" alt="akash aot" height="30" width="40" /></a>
<a href="https://akashdip2001.github.io/linktree/" target="blank"><img align="center" src="https://yt3.ggpht.com/7tPHyFi7-QyTnhpc484ZzTuRp0fZSY-CUuykvzuKdKYIwt0fmw98SWMqwRy_7pZ6LQzEYJlvXA=s88-c-k-c0x00ffffff-no-rj-mo" alt="akashdip2001" height="40" width="40" /></a>

</p>
