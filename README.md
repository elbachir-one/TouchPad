# How to set TouchPad Tapping.

1. 
`$ sudo vim /etc/X11/xorg.conf.d/30-touchpad.conf`

Section "InputClass"
	Identifier "devname"
	Driver "libinput"
		Option "Tapping" "on"
		Option "NaturalScrolling" "true"
EndSection

2. Exit and save the file and reboot your system.
