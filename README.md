# .dotfiles

Used with the following system configuration:
```
OS: Debian GNU/Linux 11 (bullseye) x86_64
Kernel: 5.10.0-14-amd64
Shell: bash 5.1.4
GNOME: 3.38.5
X.Org: 1.20.11
```

## Fix GDM wrong monitors when using NVIDIA drivers
First configure your local user monitors using the settings menu, then copy your 
configuration file to GDM user
```
$ sudo cp -v ~/.config/monitors.xml /var/lib/gdm3/.config/
$ sudo chown Debian-gdm:Debian-gdm /var/lib/gdm3/.config/monitors.xml
```