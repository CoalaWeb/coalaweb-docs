# update
sudo apt-get update

# install the 'tasksel' package so we can remove the desktop image       
sudo apt-get install tasksel

# remove the desktop image
sudo tasksel remove ubuntu-desktop

# tell tasksel to start the server image setup
sudo tasksel install server

# install the server images
sudo apt-get install linux-server linux-image-server

# remove lightdm
sudo apt-get purge lightdm

# remove all packages no longer required (~400 MB)
sudo apt-get autoremove