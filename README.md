# How to set TouchPad Tapping.

1. Create a file name 30-touchpad.conf.

`$ sudo touch /etc/X11/xorg.conf.d/30-touchpad.conf`

`$ sudo vim /etc/X11/xorg.conf.d/30-touchpad.conf`

NOTE: if xorg.conf.d does not exist, create one `$ sudo mkdir /etc/X11/xorg.conf.d` .

2. Put this code inside the file.

		Section "InputClass"
			Identifier "devname"
			Driver "libinput"
				Option "Tapping" "on"
				Option "NaturalScrolling" "true"
		EndSection

3. Save and exit the file and reboot your system.
