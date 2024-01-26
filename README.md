# vt340-notes 

Notes on setup and use of DEC VT340 terminal.

# Connect VT340 MMJ to host USB
  * [MMJ-RJ45 CABLE WITH RJ45-TO-DE-9F ADAPTER](https://decromancer.ca/dec-accessories/) - No additional null modem is needed with this cable.
  * [FTDI USB to serial](https://www.amazon.com/GearMo-Adapter-Indicators-Windows-Support/dp/B00AHYJWWG/ref=pd_rhf_ee_s_pd_sbs_rvi_d_sccl_2_5/136-3638342-9288947)
  * Set `Set-Up/GLOBAL SETUP/Comm1 Port` to `DEC-423`

# Emulation: xterm

xterm has vt340 emulation.
  * [man xterm](https://invisible-island.net/xterm/manpage/xterm.html) search for "vt340"
  * [configuring xterm](https://unix4lyfe.org/xterm/)
  * `xrdb -merge ~/.Xresources`

Example ~/.Xresources:
```
xterm*faceName: Monospace
xterm*faceSize: 14
xterm*loginshell: true
xterm*rightScrollBar: true
xterm*ScrollBar: true

xterm*termName: vt340
xterm*decGraphicsID: vt340
xterm*decTerminalID: vt340
```
