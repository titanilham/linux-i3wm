<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=30&pause=1000&color=E885F7&width=435&lines=linux+i3wm" alt="Typing SVG"/>

### Install i3wm Fedora:

```
sudo dnf install i3 i3status dmenu i3lock 
```

## Installation and configuration other programs:

### Vim or Nvim

```
sudo dnf install vim
```

```
sudo dnf install neovim
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
После установки нужно созадть файл launch.sh в /home/ilham/.config/polybar и записать туда:
```
#!/bin/sh

# Terminate already running bar instances
killall -q polybar

echo "___" | tee -a /tmp/polybar1.log /tmp/polybar2.log
polybar example 2>&1 | tee -a /tmp/polybar1.log & disown

echo "Polybar загрузился..."
```
config.ini для изменения polybar находится в /etc/polybar, его нужно скопировать в ~/.config/polybar и редактировать файл там.

### Lxappearance
```
sudo dnf install lxappearance
```
для настройки тем

темы находятся в папке - /usr/share/themes

### Flameshot

```
sudo dnf install flameshot
```
для скриншотов 

## Brightnessctl

```
sudo dnf install brightnessctl
```
для изменения яркости экрана 

## Plymouth (команды, чтобы поменять заставку запуска системы):

```
# /usr/share/plymouth/themes

plymouth-set-default-theme -l
```

```
sudo plymouth-set-default-theme -R "theme-name"
```
ссылка на темы - https://www.gnome-look.org/browse?cat=108&ord=latest

## acpi

```
sudo dnf install acpi
```
показывает процент зарядки (если работаешь в консольном режиме, что бы знать сколько осталось зарядки на ноуте)

## Мои горячие клавиши:

$mod+Print - скриншот

$mod+G - экран блокировки

$mod+P - переход в спящий режим

## Preview:

<img src="https://github.com/titanilham/linux-i3wm/blob/main/preview/2024-09-21_16-21.png?raw=true"/>

<img src="https://github.com/titanilham/linux-i3wm/blob/main/i3wm%20fedora.png?raw=true"/>

