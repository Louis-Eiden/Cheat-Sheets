# Debian Cheat Sheet

---
## **UNDER CONSTRUCTION**
---

### Table of Contents

* [Add user to sudoers](#add-user-to-sudoers)
* [Install Nvidia Driver](#install-nvidia-driver)
* [Install Bluetooth Driver](#install-bluetooth-driver)


## After Install Checklist https://www.makeuseof.com/things-to-do-after-installing-debian/

### 1. Update and upgrade

`sudo apt-get update`

`sudo apt-get upgrade`

or 

`sudo apt update && sudo apt upgrade`

### 2. [Add user to sudoers](#add-user-to-sudoers)

### 3. Install build-essential

`sudo apt-get install build-essential -y`

### Install Dash to Dock

`sudo apt install gnome-shell-extension-dash-to-dock`

---

### Install Nvidia Driver [source](#install-nvidia-driver)

#### 1. check nvidia model

`lspci | grep -i nvidia`

#### 2. Add non-free to your repositories:

`sudo nano /etc/apt/sources.list`

#### Find the lines that look like deb http://deb.debian.org/debian/ buster main and add contrib non-free at the end of each line. It should look like:

`deb http://deb.debian.org/debian/ buster main contrib non-free`

or

`echo 'deb http://deb.debian.org/debian/ buster main contrib non-free' | sudo tee /etc/apt/sources.list.d/non-free.list`

#### 3. Update package lists:

`sudo apt update`

#### 4. Install Kernel Headers

`sudo apt install linux-headers-$(uname -r)`


#### 5. Install the latest Nvidia graphics drivers on Debian 10 Buster

`sudo apt install nvidia-driver`

#### 6. Reboot your system to load the Nvidia kernel module:

`sudo reboot`

#### 7. Check if the Nvidia kernel module is loaded:

`lsmod | grep nvidia`

or

`nvidia-smi`

#

### Alternatively you can add backports to your sources.list and install the latest Nvidia drivers from there:

`sudo nano /etc/apt/sources.list`

#### Add the following line to the end of the file:

`deb http://deb.debian.org/debian buster-backports main contrib non-free`

or 

`echo 'deb http://deb.debian.org/debian buster-backports main contrib non-free' | sudo tee /etc/apt/sources.list.d/buster-backports.list`


#### Update package lists:

`sudo apt update`


#### Install the latest Nvidia graphics drivers on Debian 10 Buster from backports:

`sudo apt -t buster-backports install nvidia-driver`

#### Reboot your system to load the Nvidia kernel module:

`sudo reboot`

#### Check if the Nvidia kernel module is loaded:

`lsmod | grep nvidia`

or

nvidia-smi

#

#### 4. use nvidia-detect

sudo apt install nvidia-detect

sudo nvidia-detect

#

#### 3.7. if you have problems with the driver, you can uninstall it with:

sudo apt purge nvidia-driver 

or 

sudo apt remove --purge nvidia-*

then 

sudo apt autoremove

#### 3.8. If you want to install the latest Nvidia drivers, you can use the following PPA repository:

sudo add-apt-repository ppa:graphics-drivers/ppa

sudo apt update

sudo apt install nvidia-driver

#### 3.9. install nouveau driver (open source)

sudo apt install xserver-xorg-video-nouveau

#### 3.10. reconfigure xorg

sudo dpkg-reconfigure xserver-xorg

#### 3.11. reboot

sudo reboot

#### 3.12. check if nouveau is loaded


lsmod | grep nouveau

#### 3.13. if you have problems with the driver, you can uninstall it with:


sudo apt purge xserver-xorg-video-nouveau

or

sudo apt remove --purge xserver-xorg-video-nouveau

then

sudo apt autoremove


---

### 4. [Install Bluetooth Driver](#install-bluetooth-driver)

### 5. Install [Google Chrome](https://www.google.com/chrome/)

### 6. Install [Visual Studio Code](https://code.visualstudio.com/)

### 7. Install [Git](https://git-scm.com/)

### 8. Install [Spotify](https://www.spotify.com/us/download/linux/)

### 9. Install [Steam](https://store.steampowered.com/about/)

### 10. Install [Discord](https://discordapp.com/download)

### 11. Install [VLC](https://www.videolan.org/vlc/index.html)

### 12. Install [GIMP](https://www.gimp.org/)

### 13. Install [Inkscape](https://inkscape.org/)

### 14. Install [Blender](https://www.blender.org/)

## Add user to sudoers

### 1. Log in as Root

`su`

### 2. Add user to sudoers

`adduser <username> sudo`

or 

`usermod -aG sudo <username>`

### 3. Add user to sudoers file manually

`sudo nano /etc/sudoers`

Add `<username> ALL=(ALL) ALL` to the end of the file.


### 3. Log out and log in as user

`exit`

#

## Install Nvidia Driver

### 1. Add non-free to sources.list

`sudo nano /etc/apt/sources.list`

Add `contrib non-free` to the end of each line.

### 2. Update and install

`sudo apt-get update`

`sudo apt-get install nvidia-driver`

### 3. Reboot

`sudo reboot`

#

## Install Bluetooth Driver

### 1. Install firmware

`sudo apt-get install firmware-linux firmware-linux-nonfree`

### 2. Reboot

`sudo reboot`

or 

`sudo systemctl restart bluetooth`

or 

`sudo service bluetooth restart`

#

### Set Dash to Dock

`gsettings set org.gnome.shell.extensions.dash-to-dock dock-position BOTTOM`

#

### Install [Gnome Tweak Tool](https://wiki.gnome.org/Apps/Tweaks)

`sudo apt-get install gnome-tweak-tool`


### Install  [Docker](https://docs.docker.com/install/linux/docker-ce/debian/) and [Docker Compose](https://docs.docker.com/compose/install/)

### `sudo apt-get install docker-ce docker-ce-cli containerd.io`

### `sudo apt-get install docker-compose`

### Add user to docker group

`sudo usermod -aG docker $USER`

### Restart User Session or Reboot

### what does this do?
`su -s ${USER}`


### Install [Node.js](https://nodejs.org/en/download/package-manager/#debian-and-ubuntu-based-linux-distributions)

---

## create dash shortcut

### 1. Create .desktop file

```bash
`sudo nano /usr/share/applications/[app-name].desktop`
```

### 2. Add contents

```bash
[Desktop Entry]
Name= [app-name]
Comment=Access [app-name] on the Web
Exec=xdg-open https://web.whatsapp.com/
Terminal=false
Type=Application
Icon=[app-icon] # you can find the icon in /usr/share/icons or add your own just put the path here
Categories=Network;Application;
```

### 3. Make executable

```bash
sudo chmod +x /usr/share/applications/[app-name].desktop
```
### All in one command

```bash
echo -e "[Desktop Entry]\nName=WhatsApp Web\nComment=Access WhatsApp Web\nExec=xdg-open https://web.whatsapp.com/\nTerminal=false\nType=Application\nIcon=whatsapp\nCategories=Network;InstantMessaging;" | tee ~/.local/share/applications/whatsapp-web.desktop && chmod +x ~/.local/share/applications/whatsapp-web.desktop
