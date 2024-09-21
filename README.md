<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=30&pause=1000&color=E885F7&width=435&lines=linux+i3wm" alt="Typing SVG"/>

### Install i3wm Fedora:

```
sudo dnf install i3
```

## Installation and configuration other programs:

### Vim

```
sudo dnf install vim
```

### Rofi

```
sudo dnf install rofi
```
темы добавляются в папку - /usr/share/rofi/themes

### Nitrogen

```
sudo dnf install nitrogen
```
После установки нужно создать папку где будут находиться обои 

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
config.ini для изменения polybar находиться в /etc/polybar, его нужно скопировать в ~/.config/polybar и редактировать файл там.

### Lxappearance
```
sudo dnf install lxappearance
```
для настройки тем

### Flameshot

```
sudo dnf install flameshot
```
для скриншотов 


## Plymouth (команды, чтобы поменять заставку запуска системы):

```
# /usr/share/plymouth/themes

plymouth-set-default-theme -l
```

```
sudo plymouth-set-default-theme -R "theme-name"
```
ссылка на темы - https://www.gnome-look.org/browse?cat=108&ord=latest

## Мои горячие клавиши:

$mod+Print - скриншот

$mod+G - экран блокировки

$mod+P - переход в спящий режим

## Preview:

<img src="https://github.com/titanilham/linux-i3wm/blob/main/preview/2024-09-21_16-21.png?raw=true"/>

