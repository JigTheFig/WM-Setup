# WM-Setup

## Create an Autostart file for DWM in $HOME/.dwm/autostart.sh
```
#! /bin/bash 
compton &
nitrogen --restore &
dwmblocks &
``` 
Make sure it's executable, run chmod +x. 
## Dependencies & Programs
```
libxft
ttf-hack
ttf-joypixels
st
dmenu
tabbed
pulseeffects
```
AUR Packages
```
nerd-fonts-complete
libxft-bgra
picom-jonaburg-git
```
## Install
```
make
sudo make install
```
## Add DWM to .xinitrc
```
exec dwm
```
## Keybindings
```
MODKEY + RETURN
opens terminal (alacritty is the terminal but can be easily changed)


MODKEY + SHIFT + RETURN
opens run launcher (dmenu is the run launcher but can be easily changed)


MODKEY + SHIFT + c
closes window with focus


MODKEY + SHIFT + r
restarts dwm


MODKEY + SHIFT + q
quits dwm


MODKEY + 1-9
switch focus to workspace (1-9)


MODKEY + SHIFT + 1-9
send focused window to workspace (1-9)


MODKEY + j
focus stack +1 (switches focus between windows in the stack)


MODKEY + k
focus stack -1 (switches focus between windows in the stack)


MODKEY + SHIFT + j
rotate stack +1 (rotates the windows in the stack)


MODKEY + SHIFT + k
rotate stack -1 (rotates the windows in the stack)


MODKEY + h
setmfact -0.05 (expands size of window)


MODKEY + l
setmfact +0.05 (shrinks size of window)


MODKEY + .
focusmon +1 (switches focus next monitors)


MODKEY + ,
focusmon -1 (switches focus to prev monitors)
```
## PulseEffects Presets
```
bash -c "$(curl -fsSL https://raw.githubusercontent.com/JackHack96/PulseEffects-Presets/master/install.sh)"
```
