# flatpak-indicator-kdeconnect #

flatpak package for bajoja's [indicator-kdeconnect](https://github.com/Bajoja/indicator-kdeconnect).

for now it's don't send sms, files or browser the devices 
but you can see the device notifications, battery and uses the "find my phone" options.

# Todos #

 · <del>run indicator-kdeconnect-settings(see, [#2](https://github.com/MrMarukesu/flatpak-indicator-kdeconnect/issues/2)).</del> <br>
 · add "dev" branch .json. <br>
 · <del>test with org.kde.kdeconnect flatpak.</del> (run) <br>
 · <del>make dbus run the indicator(see, [#1](https://github.com/MrMarukesu/flatpak-indicator-kdeconnect/issues/1)).</del> <br>
 · <del>exports the indicator icons(see, [#3](https://github.com/MrMarukesu/flatpak-indicator-kdeconnect/issues/3)).</del> <br>
 · <del>add python to depedences? (see, [#4](https://github.com/MrMarukesu/flatpak-indicator-kdeconnect/issues/4)).</del>
 

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
for execute, run:
```
$ flatpak run com.github.bajoja.indicator-kdeconnect
```
and
```
$ flatpak run --command=indicator-kdeconnect-settings com.github.bajoja.indicator-kdeconnect
```
if you wanna run the settings from terminal
