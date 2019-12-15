# My-rxvt-config
My configuration for the rxvt terminal
![What it looks like](https://raw.githubusercontent.com/BeanGreen247/My-rxvt-config/master/screen.png)

## Installation
To install rxvt run
```bash
sudo apt install rxvt
```
Get the config and apply it
```bash
wget -O ~/.Xresources https://raw.githubusercontent.com/BeanGreen247/My-rxvt-config/master/Xresources
sudo xrdb -merge ~/.Xresources
```
## The config
```bash
URxvt.font: xft:mono:bold:size=10
URxvt.clipboard.autocopy: true
URxvt.keysym.M-c: perl:clipboard:copy
URxvt.keysym.M-v: perl:clipboard:paste
URxvt.scrollBar: false
URxvt.saveLines:0
URxvt.transparent: true
URxvt.shading:20

! special
*.foreground:   #ffffff
*.background:   #1d1f21
*.cursorColor:  #ffffff

! black
*.color0:       #2e3139
*.color8:       #373b41

! red
*.color1:       #bc1919
*.color9:       #ff0000

! green
*.color2:       #008000
*.color10:      #00b92c

! yellow
*.color3:       #ffb600
*.color11:      #ffb600

! blue
*.color4:       #0066ff
*.color12:      #0066ff

! magenta
*.color5:       #ff00cb
*.color13:      #ff00cb

! cyan
*.color6:       #00ffdd
*.color14:      #00ffdd

! white
*.color7:       #00ffe9
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
