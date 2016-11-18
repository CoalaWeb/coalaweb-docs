FTP
Install FTP to allow transferring files to and from your Raspberry Pi.

sudo apt-get install vsftpd

Now we can begin the configuration process. First have to edit the vsftpd.config file. To edit the file use the following command:

sudo nano /etc/vsftpd.conf

Find and edit the following lines as specified:

Change anonymous_enable=YES to anonymous_enable=NO,
Uncomment local_enable=YES
Uncomment write_enable=YES

The last change we will make is the adding of the following line to the bottom of the file. This will force the display of hidden files and folders that are preceded by a "." or "..". This will help stop accidental deletions or overwriting of hidden files such as .htaccess.
force_dot_files=YES




*to uncomment, remove the pound sign (#) in front of the specified line

exit the editing interface by pressing ctrl+X, type y to confirm the changes and press enter to save the file path. 

Restart the FTP service with the following command:

sudo service vsftpd restart

## PHPMyAdmin

### About phpMyAdmin

phpMyAdmin is a free software to work with MySQL on the web—it provides a convenient visual front end to the capabilities of MySQL.
Setup

### Install PHPMyAdmin

Start off by downloading and installing the program with apt-get.

sudo apt-get install phpmyadmin

When phpmyadmin prompts you to choose a server (either apache or lighttpd) hit tab, and select neither one.

Select none

Image

During the installation, phpmyadmin will ask you if you want to configure the database with dbconfig. Go ahead and choose yes.

image

Input MySQL’s database password when prompted and click ok.

image

Input phpmyadmin password to register with the databse server and then confirm it.

image.

### Step Two Configure phpMyAdmin

You now have phpMyAdmin installed on your server. In order to access it, you need to take one more step.

Create a symbolic link between phpMyAdmin and your site’s directory. If you were using the previous tutorial, it may be still located in the nginx default directory, otherwise link it with the appropriate place:

sudo ln -s /usr/share/phpmyadmin/ /usr/share/nginx/www

Restart nginx:

sudo service nginx restart

You should now be able to access phpMyAdmin by going to yourdomain/phpmyadmin. The screen will look like this.

image

Log in with your MySQL username and password.
