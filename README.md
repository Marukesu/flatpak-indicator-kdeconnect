# flatpak-indicator-kdeconnect #

flatpak package for bajoja's [indicator-kdeconnect](https://github.com/Bajoja/indicator-kdeconnect).

# Todos #

 · run indicator-kdeconnect-settings(see, [#2](https://github.com/MrMarukesu/flatpak-indicator-kdeconnect/issues/2)). <br>
 · add "dev" branch .json. <br>
 · <del>test with org.kde.kdeconnect flatpak.</del> (run) <br>
 · make dbus run the indicator(see, [#1](https://github.com/MrMarukesu/flatpak-indicator-kdeconnect/issues/1)).

# How test #

Firstly you need flatpak and flatpak-builder installed in you computer. 
for ubuntu-based disto, her is installed with this command:
```
$ sudo add-apt-repository ppa:alexlarsson/flatpak
$ sudo apt update
$ sudo apt install flatpak
```
See http://flatpak.org/getting.html for installations methods for others distros.
 
#

For now, if you wanna test this flatpak you need compile it from flatpak-builder with this commands, 
inside of this directory run:
```
$ flatpak-builder --repo=~/repo indicator-kdeconnect com.github.bajoja.indicator-kdeconnect.json
$ flatpak remote-add --no-gpg-verify repo ~/repo
$ flatpak install repo com.github.bajoja.indicator-kdeconnect.json
```
and for execute, run:
```
$ flatpak run com.github.bajoja.indicator-kdeconnect
```
