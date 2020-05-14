##### Configurazione per GNOME

```bash
sudo pacman -S gnome
sudo pacman -R gnome-documents gnome-music epiphany gnome-books
sudo systemctl enable gdm.service

sudo localectl set-locale LANG=it_IT.UTF-8
sudo pacman -S noto-fonts noto-fonts-emoji ttf-croscore ttf-roboto

sudo pacman -S cups system-config-printer nss-mdns
sudo systemctl enable org.cups.cupsd.service && systemctl start org.cups.cupsd.service
sudo systemctl enable avahi-daemon.service && systemctl start avahi-daemon.service
sudo nano /etc/nsswitch.conf
	mdns_minimal [NOTFOUND=return] resolve [...]

yay -S arc-gtk-theme-jnsh-git papirus-icon-theme # Dopodiché configura il sistema cone le icone e i temi corretti, per Gnome-Shell prima cambia la dimensione dei font a 10 e esegui lo script per GDM3
```

##### Configurazione per XFCE4

```bash
sudo pacman -S xfce4 xfce4-goodies udisks2 udevil exfat gvfs lightdm lightdm-gtk-greeter
sudo systemctl enable lightdm.service

sudo localectl set-locale LANG=it_IT.UTF-8
sudo pacman -S noto-fonts noto-fonts-emoji ttf-croscore ttf-roboto cantarell-fonts

sudo pacman -S cups system-config-printer nss-mdns
sudo systemctl enable org.cups.cupsd.service && systemctl start org.cups.cupsd.service
sudo systemctl enable avahi-daemon.service && systemctl start avahi-daemon.service
sudo nano /etc/nsswitch.conf
	mdns_minimal [NOTFOUND=return] resolve [...]

yay -S arc-gtk-theme-jnsh-git papirus-icon-theme # Dopodiché configura il sistema cone le icone e i temi corretti

sudo pacman -S geany xarchiver xpdf galculator audacious zip unzip gparted
yay -S mugshot
```

##### App Consigliate

```bash
sudo pacman -S libreoffice-fresh libreoffice-fresh-it vlc
yay -S google-chrome spotify
```

Consiglio l'utilizzo del wallpaper [default.png](default.png)
