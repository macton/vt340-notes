# vt340-notes 

Notes on setup and use of DEC VT340 terminal.

# Emulation: xterm

xterm has vt340 emulation.
  * (man xterm)[https://invisible-island.net/xterm/manpage/xterm.html] search for "vt340"
  * (configuring xterm)[https://unix4lyfe.org/xterm/]

~/.Xresources:
```
! Use a truetype font and size.
xterm*faceName: Monospace
xterm*faceSize: 14

! Every shell is a login shell by default (for inclusion of all necessary environment variables)
xterm*loginshell: true


! right hand side scrollbar...
xterm*rightScrollBar: true
xterm*ScrollBar: true

xterm*termName: vt340
xterm*decGraphicsID: vt340
xterm*decTerminalID: vt340
```
