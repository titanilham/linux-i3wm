# linux i3wm

### Install i3wm Fedora:

```
sudo dnf install i3
```

## Installing other programs:

### Rofi

```
sudo dnf install rofi
```
### Nitrogen

```
sudo dnf install nitrogen
```
После установки нужно создать папку где будуд находиться обои 

```
# ~/.config/i3/config

exec --no-startup-id nitrogen /home/ilham/Изображения/wallpaper --restore; sleep 1
```

### Picom

```
sudo dnf install picom
```

### Nemo

```
sudo dnf install nemo
```

### Xscreensaver

```
```
### Polybar

```
sudo dnf install polybar
```
После утсановки нужно созадть файл launch.sh в /home/ilham/.config/polybar и записать туда:
```
#!/bin/sh

# Terminate already running bar instances
killall -q polybar

echo "___" | tee -a /tmp/polybar1.log /tmp/polybar2.log
polybar example 2>&1 | tee -a /tmp/polybar1.log & disown

echo "Polybar загрузился..."
```
config.ini для изменения polybar находиться в /etc/polybar



