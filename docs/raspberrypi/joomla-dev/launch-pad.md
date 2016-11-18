Write Image

# Which device? run without your card plugged in
df -h
# now plug it in run the command again and note down the new drive that appears in the list

# The 1 denotes a partition so the later we will only be interested in the name before that so for example sdc1 is sdc partition 1

# umount it (all partitions if more than one)
umount /dev/sdc1

# change to the directory where the extracted img that was downloaded to
cd /home/steve/resources/raspberry/

# write the image to the drive we established earlier minus the partition number
sudo dd bs=4M 2015-02-16-raspbian-wheezy.img of=/dev/sdc

# it will take some time but when it finishes run 
sync
# this will ensure the write cache is flushed and that it is safe to unmount your SD card. Then remove the SD card from the card reader and plug it into your pi.

Get started with our pi
Now that we have a new raspberry pi connected to a monitor, keyboard, mouse and network via ethernet it’s time to do some initial setup before we access it through the network via SSH.

tip: sudo raspi-config anytime to get back to the config page

Expand file system - You should receive a message that it will take effect next reboot
Change password
I personally overclock it to medium but its up to you
Advanced - update
Finish

# Now lets configure the network interface to use a static IP. I will be using the ethernet port on my raspberry pi because it’s faster and more eleiable plus my pi will be functioning headless (no monitor, keyboard or mouse) so it can sit nicely next to my router.

sudo nano /etc/network/interfaces

#Firstly change the word dhcp next the iface eth0 to static
iface eth0 inet static

# then under that enter the follow lines
address 192.168.1.104
netmask 255.255.255.0
network 192.168.1.0
broadcast 192.168.1.255
gateway 192.168.1.1

Change the username in your PI
usermod command won't run if there are any processes of the to-be-changed user running on the machine when the command is run.
If your on console of the pi there is a way to get around this without having to make another user (or set a pw on root):
Assuming nothing else is running with your username other then the shell on the console - no X session, no ssh login, etc:
exec sudo -s
cd /
usermod -l newname -d /home/newname -m oldname


The reason this works:
sudo -s tells sudo that instead of just running on command as another user that it should run new shell as the given user
exec tells the shell that instead of spawning off a new process when it runs a command (hence leaving the shell process running as the login user) that the shell should overwrite itself with the new process - this means that when exec ed command ends the shell is gone - in the case of a login shell that equates to disconnecting from the login
the cd / is optional. At minimum, things get a bit confusing if you move a dir your in (your login starts out sitting in the user pi home dir) but sometimes will cause a fail, better safe then sorry.
Therefor with exec sudo -s your overwriting your shell with a new shell that has been created as a different user.
P.S. be sure to give usermod -d a full path or you'll end up moving the account's home to somewhere you don't expect (and have a bogus directory entry in passwd)

Now lets shut it down and make a copy so we dont have to go through that again to get to our initial setup.
sudo shutdown -h now

Now you should be able to connect to your pi through your network using ssh. Let give it a try with the following command. Remeber to substitue coalaweb with the username you change to in the last step

ssh coalaweb@192.168.1.104

You will be asked to accept the digital certificate eneter yes and it will remeber it for next time your connect.
