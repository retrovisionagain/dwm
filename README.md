# Simple DWM setup
![Screenshot 1](https://github.com/retrovisionagain/dwm/blob/main/dwm.png)
![Screenshot 2](https://github.com/retrovisionagain/dwm/blob/main/busy-dwm.png)

This is my dwm configuration files. Here you'll find:
- dwm
- dwmblocks
- alacritty

## Installation
```bash
git clone https://github.com/retrovisionagain/dwm
cd dwm
cd dwmdir
make && sudo make install
cd ../dwmblocks
make && sudo make install
cd ..
# This will overwrite your previous configuration of alacritty
cp -r alacritty ~/.config
cp startdwm.sh /usr/local/bin/
```

If you use a display manager
```bash
sudo cp dwm.desktop /usr/local/share/xsessions/
```
If you don't
```bash
echo "exec /usr/local/bin/startdwm.sh" >> ~/.xinitrc
```
