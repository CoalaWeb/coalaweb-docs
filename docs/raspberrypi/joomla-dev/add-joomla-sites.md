# Additonal Joomla Sites

This guide is assuming the following:
You have complete the previous guides in this series.
You are adding an additional Joomla site.

### Things to note:
-   For this guide our Joomla website will be called j34-dev3
-   We are using a Rapberry Pi 2
-   We are using an Ubuntu

## Step 1 Preparation

### Create new Nginx Server Block

First lets create a new Server Block File by copying the first one you created in our earlier guide.

    sudo cp  /etc/nginx/sites-available/j34-dev1 /etc/nginx/sites-available/j34-dev3

Now lets open our new file and makes some changes.

    sudo nano  /etc/nginx/sites-available/j34-dev3

First remove the server next to this line.

    listen 80;

Update the server name to the new site name in our case it will become.

    server_name j34-dev3;

Lastly change the error log location to reflect our new site name so this line will become.

    error_log /var/log/nginx/j34-dev3.error.log;

Feel free to research any of the settings I have chosen but keep in mind we are just going to use this server for development not for live sites.

Note: Each Nginx statement must end with a semi-colon (;), so check each of your lines if you are running into problems.


### Enable new Server Block

You now have your server block created, we need to enable it. We can do this by creating symbolic links from this file to the sites-enabled directory, which Nginx reads from during startup.

We can create these links by typing the command below making sure to replace the name with yours:

    sudo ln -s /etc/nginx/sites-available/j34-dev3 /etc/nginx/sites-enabled/

### Restart Nginx Server

Now let restart our Nginx server and check for any issues.

    sudo service nginx restart


### Get Joomla

Step 1
First switch to the downloads directory you created in an earlier guide.

    cd /home/coalaweb/downloads

Now lets get the link to the latest version of Joomla from http://www.joomla.org/download.html Under the Download button use the Alternative download location link.

image

Next copy the link for the latest Stable Full version that finishes in **tar.gz**

image

Then in the terminal making sure you are currently in your downloads directory run this command.

    wget http://joomlacode.org/gf/download/frsrelease/20021/162256/Joomla_3.4.1-Stable-Full_Package.tar.gz

You will see the progress of the download in the terminal window.

image

When it has finished move onto the next step.

Step 2 
Create website directory

Now lets create a directory for our new website.

    sudo mkdir /usr/share/nginx/www/j34-dev3

Then make sure the permissions are right for the new directory

    sudo chown -R www-data:www-data /usr/share/nginx/www/j34-dev3
    sudo chmod -R 775 /usr/share/nginx/www/j34-dev3
    sudo chmod -R g+rwx /usr/share/nginx/www/j34-dev3

If you aren’t already change to the directory you have your copy of Joomla in

    cd /home/coalaweb/downloads/

This command unzip it into the chosen directory making sure the last part is to the correct location

$ sudo tar zxvf Joomla_3.4.1-Stable-Full_Package.tar.gz -C /usr/share/nginx/www/j34-dev3

# let make sure the permission are right on the extract files

sudo chown -R www-data:www-data /usr/share/nginx/www
sudo chmod -R 775 /usr/share/nginx/www
sudo chmod -R g+rwx /usr/share/nginx/www

# MySQL

Now we need to add a new database for our addtianl Joomla webiste

#First log into MySql using the root user you create in the previous guide.

sudo mysql -uroot -hlocalhost -p

# Now create the database with the following command updating the name as needed.

CREATE DATABASE `j34-dev3`;

# when you have finished you can disconnect from MySql like this.

exit

run Joomla installer script
