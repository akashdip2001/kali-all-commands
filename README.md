# kali-all-commands
all imp. commands of KALI LINUX. This repositry helps to install, Uninstall, WIFI peoblams, all usefull apps .... etc. 


# WIFI Connect but Not working 
    sudo systemctl status systemd-resolved.service 
    sudo systemctl restart systemd-resolved.service (only this )
    sudo systemctl status systemd-resolved.service 

# Turn ON Bluetooth
service bluetooth restart

# install Softwers in KALI Linux ---
    sudo dpkg -i *.deb  ( normal .deb file install command )
    ./configure  ---  make install ( install Python in Kali command )
 	      
   


# uninstall  --- 
               dpkg --list
               sudo apt --purge remove gimp
               sudo apt remove gimp
               sudo apt-get autoremove
               sudo apt purge --auto-remove gimp
               sudo apt clean
               
# snap install but not Working ---
         systemctl enable --now snapd.apparmor


# all imp. Softwers in KALI 
    kdeconnect
    freecad
    shotcut   ---- DaVinci
    gimp      ---- rawtherapee 
    simplescreenrecorder
    audacity
    handbrake
    codeblocks
    blender
    freeDownloadManager
    telegram
    ktouch
    virtualbox
    terminator
    edge
    audacious (mp3)


# Delet File --  
     rm -rfv ssr
