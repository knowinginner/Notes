# Notes
Opensuse install

rm libreoffice
rm firefox

media repo

sudo zypper install opi
opi packman

## WINDOWS TILLING

https://github.com/MX-Linux/desktop-defaults-xfce-mx/blob/main/dd-mx-xfce-desktop/skel/.config/xfce4/xfconf/xfce-perchannel-xml/xfce4-keyboard-shortcuts.xml

---

## BRAVE ADDONS

https://chromewebstore.google.com/detail/gofullpage-full-page-scre/fdpohaocaechififmbbbbbknoalclacl

https://chromewebstore.google.com/detail/xbrowsersync/lcbjdhceifofjlpecfpeimnnphbcjgnc

https://chromewebstore.google.com/detail/bitwarden-free-password-m/nngceckbapebfimnlniiiahkandclblb

https://chromewebstore.google.com/detail/web-developer/bfbameneiokkgbdmiekhjnmfkcnldhhm

https://chromewebstore.google.com/detail/web-developer-tool-for-ch/ghenifimhcdihapkceohjpgiabidpgji

https://chromewebstore.google.com/detail/video-downloadhelper/lmjnegcaeklhafolokijcfjliaokphfk

---

ICONS

git clone https://github.com/zayronxio/Mojave-CT.git

---

THEME

git clone https://github.com/vinceliuice/WhiteSur-gtk-theme.git --depth=1

cd WhiteSur-gtk-theme

./install.sh -c Dark -c Light


---

NORDVPN

https://nordvpn.com/download/linux/
https://support.nordvpn.com/Connectivity/Linux/1325531132/Installing-and-using-NordVPN-on-Debian-Ubuntu-Raspberry-Pi-Elementary-OS-and-Linux-Mint.htm

sh <(curl -sSf https://downloads.nordcdn.com/apps/linux/install.sh)


nordvpn login

nordvpn connect

nordvpn c double_vpn

nordvpn set threatprotectionlite on

nordvpn set killswitch on

nordvpn set autoconnect on

---

FIREWALL

---

APPS 

hugo go corepack rofi htop npm libwebp-tools optipng jpegoptim

sudo npm install -g pnpm

sudo npm install -g postcss postcss-cli autoprefixer

sudo zypper install distrobox # pulls in docker by default
sudo groupadd docker; sudo usermod -aG docker $USER # you should re-login with the user for changes to take effect
sudo systemctl enable --now docker
distrobox enter

sudo flatpak install flathub com.brave.Browser

sudo flatpak install flathub net.mullvad.MullvadBrowser

sudo flatpak install flathub org.standardnotes.standardnotes

sudo flatpak install flathub com.visualstudio.code-oss

sudo flatpak install flathub com.vscodium.codium

sudo flatpak install flathub org.freefilesync.FreeFileSync

sudo flatpak install flathub org.gimp.GIMP

sudo flatpak install flathub org.libreoffice.LibreOffice

sudo flatpak install flathub com.discordapp.Discord

sudo flatpak install flathub nz.mega.MEGAsync

sudo flatpak install flathub org.videolan.VLC

sudo flatpak install flathub org.gnome.meld

sudo flatpak install flathub com.github.Murmele.Gittyup

sudo flatpak install flathub xyz.xclicker.xclicker

icedrive
pcloud

---

MEGA-CMD

https://mega.io/cmd

https://github.com/meganz/MEGAcmd/blob/master/UserGuide.md

wget https://mega.nz/linux/repo/openSUSE_Tumbleweed/x86_64/megacmd-openSUSE_Tumbleweed.x86_64.rpm && sudo zypper install "$PWD/megacmd-openSUSE_Tumbleweed.x86_64.rpm"

mega-cmd login

sync /path/to/local/folder /folder/in/mega
sync /home/fedora/MEGA/ /docs/


https://github.com/meganz/MEGAcmd/issues/499

$HOME/.config/systemd/user/mega-cmd.service

[Unit]
Description=MEGA cmd server
After=network.target

[Service]
Type=simple
ExecStart=/usr/bin/mega-cmd-server
Restart=always

[Install]
WantedBy=default.target


systemctl --user --daemon-reload
systemctl --user enable mega-cmd.service
systemctl --user start mega-cmd.service
systemctl --user status mega-cmd.service

---

## ROFI

git clone --depth=1 https://github.com/adi1090x/rofi.git

cd rofi

chmod +x setup.sh

sh setup.sh

/home/fedora/.config/rofi/launchers/type-2/launcher.sh

---

KEYBOARD SHORTCUTS

