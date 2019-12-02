# My-rxvt-config
My configuration for the rxvt terminal
![What it looks like](https://raw.githubusercontent.com/BeanGreen247/My-rxvt-config/master/Screenshot%20from%202019-12-02%2020-36-33.png)
## The config
```bash
URxvt.font: xft:mono:bold:size=10
URxvt.clipboard.autocopy: true
URxvt.keysym.M-c: perl:clipboard:copy
URxvt.keysym.M-v: perl:clipboard:paste
URxvt.scrollBar: false

! special
*.foreground:   #ffffff
*.background:   #000000
*.cursorColor:  #ffffff

! black
*.color0:       #2e3139
*.color8:       #373b41

! red
*.color1:       #bc1919
*.color9:       #ff0000

! green
*.color2:       #008000
*.color10:      #00bd68

! yellow
*.color3:       #fbff00
*.color11:      #fbff00

! blue
*.color4:       #005397
*.color12:      #005397

! magenta
*.color5:       #73527d
*.color13:      #73527d

! cyan
*.color6:       #009480
*.color14:      #009480

! white
*.color7:       #37928a
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
