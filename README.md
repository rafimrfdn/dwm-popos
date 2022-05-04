# dwm-popos
My DWM build for PopOS or Debian live Standart ISO LTS.

![dwm-debian-lts-xfce](https://github.com/rafimrfdn/dwm-popos/blob/main/dwm-debian-with-xfce-lts.png)

## For Debian standard / XFCE iso

Install these apps first to build this DWM:

```
sudo apt install neovim git kitty wget rofi picom fonts-terminus libx11-dev libxft-dev libxinerama-dev build-essential make libharfbuzz-dev zsh zsh-autosuggestions zsh-syntax-highlighting
```

The iso included Firefox-esr, and you can still use Thunar file manager instead of install another file manager like Pcmanfm.

To launch DWM on your system, just create a desktop file on `/usr/share/xsessions/` named *dwm.desktop* then fill with this line

```
  [Desktop Entry]                                                                
  Encoding=UTF-8                                                                 
  Name=Dwm                                                                       
  Comment=Dynamic window manager                                                 
  Exec=dwm                                                                       
  Icon=dwm                                                                       
  Type=XSession
```
So at the next reboot you can choose DWM from LightDM login session.

## For PopOS

Please add these apps :

```
sudo apt install pcmanfm xarchiver kitty etc...
```

If you want to activate Gnome apps and feature, just edit `.xinitrc` then add **exec gnome-session**

## Additional setting for this DWM build

Just edit the `config.h` file then change the line 77 into your system username.

## About this build

This DWM based on DWM 6.2 with some usefull pathces. 

You can read the keybind from `config.h` file.

Hope you enjoy
