Raspberry Pi Auto Start and Read Only SD Scripts

nano ~/.config/lxsession/LXDE-pi/autostart

https://www.raspberrypi.org/forums/viewtopic.php?f=63&t=199672

https://www.raspberrypi-spy.co.uk/2015/02/how-to-autorun-a-python-script-on-raspberry-pi-boot/

sudo nano /etc/profile

sudo python3 /home/pi/ruff-wavs/shufflewavdemo.py &

sudo /root/reboot-to-readonly-mode.sh

sudo /root/reboot-to-writable-mode.sh

-----
-Rehoot auto
-https://www.raspberrypi.org/forums/viewtopic.php?t=118069

pi@raspberrypi:~ $ sudo nano /etc/cron.d/reboot

@reboot /sbin/shutdown -r 23:59
---------
https://www.raspberrypi.org/forums/viewtopic.php?t=202549

To run after the GUI starts at startup try putting the relevant command in ~/.config/lxsession/LXDE-pi/autostart
Type sudo nano ~/.config/lxsession/LXDE-pi/autostart in terminal
Eg. To run a python script use...
@sudo /usr/bin/python /home/pi/filename.py
Press CTRL & X, then Y to save.
To Make the file executable with sudo chmod +x filename.py
It will run after the gui starts

---------


Nayme better

https://www.raspberrypi.org/forums/viewtopic.php?t=126264

 