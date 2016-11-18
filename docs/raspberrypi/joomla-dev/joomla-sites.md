Install Joomla

#Next we will need to create a directory where you will keep your Joomla files temporarily:

mkdir /home/coalaweb/downloads

#Switch into the directory:

cd /home/coalaweb/downloads

#now lets the link to the latest version of Joomla from http://www.joomla.org/download.html
under the Download button use the Alternative download location link.

image

Next copy the link for the latest Stable Full version that finishes in tar.gz

image

wget http://joomlacode.org/gf/download/frsrelease/20021/162256/Joomla_3.4.1-Stable-Full_Package.tar.gz


#If you are following on from the previous guides in this series then you should already have the following directories created.

/usr/share/nginx/www/j34-dev1
/usr/share/nginx/www/j34-dev2

# If you are back to create an additional one just use the same process

sudo mkdir /usr/share/nginx/www/j34-dev3

# then make sure the permissions are right for your new site directory

sudo chown -R www-data:www-data /usr/share/nginx/www/j34-dev3
sudo chmod -R 775 /usr/share/nginx/www/j34-dev3
sudo chmod -R g+rwx /usr/share/nginx/www

# If you aren’t already change to the directory you have your copy of Joomla in

 cd /home/coalaweb/downloads/

#This command unzip it into the chosen directory making sure the last part is to the correct location

$ sudo tar zxvf Joomla_3.4.1-Stable-Full_Package.tar.gz -C /usr/share/nginx/www/j34-dev1

# run the same command to extract Joomla to any other location you want to install it to.

$ sudo tar zxvf Joomla_3.4.1-Stable-Full_Package.tar.gz -C /usr/share/nginx/www/j34-dev2
$ sudo tar zxvf Joomla_3.4.1-Stable-Full_Package.tar.gz -C /usr/share/nginx/www/j34-dev3

# let make sure the permission are right on the extract files

sudo chown -R www-data:www-data /usr/share/nginx/www
sudo chmod -R 775 /usr/share/nginx/www
sudo chmod -R g+rwx /usr/share/nginx/www

MySQL
If you have been following on from the other guides in this series you should already have two databases created called.

j34-dev1
j34-dev2

If you adding an additional webiste use the same steps to create an additional database.

#First log into MySql using the root user you create in the previous guide.

sudo mysql -uroot -hlocalhost -p

# Now create the database with the following command updating the name as needed.

CREATE DATABASE `j34-dev3`;

# when you have finished you can disconnect from MySql like this.

exit

run Joomla installer script
