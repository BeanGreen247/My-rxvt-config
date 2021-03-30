# My-rxvt-config
My configuration for the rxvt terminal
![What it looks like](https://raw.githubusercontent.com/BeanGreen247/My-rxvt-config/master/screen.png)

## Installation
To install rxvt run
```bash
sudo apt install -y rxvt wget
```
Get the config and apply it
```bash
wget -O ~/.Xresources https://raw.githubusercontent.com/BeanGreen247/dotfiles/master/rxvt/Xresources
sudo xrdb -merge ~/.Xresources
```
## The config
```bash
URxvt.clipboard.autocopy: true
URxvt.scrollBar: false
URxvt.saveLines:10000
URxvt.font: xft:Hermit:size=9
URxvt.geometry: 80x35

! special
*.foreground:   #919191
*.background:   #000000
*.cursorColor:  #919191

! black
*.color0:       #303030
*.color8:       #5e5e5e

! red
*.color1:       #c10023
*.color9:       #ff8781

! green
*.color2:       #a83334
*.color10:      #ffa095

! yellow
*.color3:       #b51d2c
*.color11:      #ff948b

! blue
*.color4:       #8c4b46
*.color12:      #feb2aa

! magenta
*.color5:       #7d534f
*.color13:      #ebbbb5

! cyan
*.color6:       #9a413d
*.color14:      #ffaaa0

! white
*.color7:       #c6c6c6
*.color15:      #ffffff

!! Common Keybinds for Navigations
URxvt.keysym.Shift-Up: command:\033]720;1\007
URxvt.keysym.Shift-Down: command:\033]721;1\007
URxvt.keysym.Control-Up: \033[1;5A
URxvt.keysym.Control-Down: \033[1;5B
URxvt.keysym.Control-Right: \033[1;5C
URxvt.keysym.Control-Left: \033[1;5D

!! Copy Paste & Other Extensions
URxvt.perl-ext-common: default,clipboard,url-select,keyboard-select
URxvt.copyCommand: xclip -i -selection clipboard
URxvt.pasteCommand: xclip -o -selection clipboard
URxvt.keysym.M-c: perl:clipboard:copy
URxvt.keysym.M-v: perl:clipboard:paste
URxvt.keysym.M-C-v: perl:clipboard:paste_escaped
URxvt.keysym.M-Escape: perl:keyboard-select:activate
URxvt.keysym.M-s: perl:keyboard-select:search
URxvt.keysym.M-u: perl:url-select:select_next
URxvt.urlLauncher: firefox
URxvt.underlineURLs: true
URxvt.urlButton: 1
```
