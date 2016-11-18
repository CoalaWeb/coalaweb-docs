Install ngnix

# First lets do a little bit of maintenance to make sure our packages are upto date and our system is clean of unneeded fluff.

Note: this can take some time

sudo sh -c "apt-get update;apt-get dist-upgrade;apt-get autoremove;apt-get autoclean"

# now install Nginx first

sudo apt-get install nginx

image

#now let try and start it if it hasn’t already to check its working as expected.

sudo /etc/init.d/nginx start

image

# now try our IP in the browser

image

Create our site directories

# By default, Nginx on Ubuntu 14.04 has one server block enabled by default. It is configured to serve documents out of a directory at:

/usr/share/nginx/www

Note: for production servers it’s normally a good idea to move your web server root to /var/www but in our case we are only using it for development purposes so I’m leaving everything in their default locations.


First, we need to create the necessary directories. We can do this with the following commands.

sudo mkdir /usr/share/nginx/www/j34-dev1
sudo mkdir /usr/share/nginx/www/j34-dev2

groups and permissions

# Let check what groups our user belong to.

groups coalaweb

image

# the first group is the primary and for our development server we want our user to belong to the www-data group and have it set as their primary group. This will help with permissions and access to the web directories.

# We can add our user to www-data like this

sudo usermod -a -G www-data coalaweb

# now we can make it the primary group like this

sudo usermod -g www-data coalaweb

image

# change ownership for www folder to the nginx user (www-data)

sudo chown -R www-data:www-data /usr/share/nginx/www
sudo chmod -R 775 /usr/share/nginx/www

# I actually give group write permissions as well, for users which need to modify content, such as users used to deploy code,

sudo chmod -R g+rwx /usr/share/nginx/www

Create Sample Pages for Each Site
Now that we have our directory structure set up, let's create a default page for each of our sites so that we will have something to display.

Create an index.html file in your first domain:

sudo nano /usr/share/nginx/www/j34-dev1/index.html


Inside the file, we'll create a really basic file that indicates what site we are currently accessing. It will look like this:
<html>
    <head>
        <title>Welcome to your Raspberry Pi host website!</title>
    </head>
    <body>
        <h1>Success!  The j34-dev1 server block is working!</h1>
    </body>
</html>


Exit the editing interface by pressing ctrl+X, type y to confirm the changes and press enter to save the file path.

Since the file for our second site is basically going to be the same, we can copy it over to our second document root like this:

sudo cp  /usr/share/nginx/www/j34-dev1/index.html  /usr/share/nginx/www/j34-dev2/index.html


Now, we can open the new file in our editor and modify it so that it refers to our second website

nano  /usr/share/nginx/www/j34-dev1/index.html


<html>
    <head>
        <title>Welcome to Test.com!</title>
    </head>
    <body>
        <h1>Success!  The test.com server block is working!</h1>
    </body>
</html>


Exit the editing interface by pressing ctrl+X, type y to confirm the changes and press enter to save the file path. You now have some pages to test both of your sites with.



Configure Nginx

Before we start I will explain a bit about what files we will be altering to get Ngnix working for us.

# To make it easy to follow I will refer to the following file as the Nginx configuration file where we will be making changes that will affect the overall functioning of the Ngnix server.

/etc/nginx/nginx.conf

For the individual installation of Joomla (virtual hosts) that we will be creating server block files for each of the sites. For this example we will be creating two sites and their associated configuration files will be the following.

/etc/nginx/sites-available/j34-dev1
/etc/nginx/sites-available/j34-dev2

# Nginx configuration file
Rather than going through un commenting and adding lines of code to this file I will be creating a backup of it for future reference and then replacing it with the code example below.

# first lets make a backup of the file so you always have a reference to the original settings

sudo cp /etc/nginx/nginx.conf /etc/nginx/nginx.conf.bak

# Now I will show you a little Nano trick for clear the old file content and replacing it with our new code.

# Lets start by opening the current file
sudo nano /etc/nginx/nginx.conf

# now move the cursor to the top left corner and press alt a this will mark that spot. Now just use the down arrow and you should see all the text being highlighted, keep scrolling down until you hit the bottom and then use the CTRL k combination to cut it.

Now make a copy of the code below with the standard highlight and copy combination and then in the Nano window right click and past it.

CODE

# Virtual Hosts

Now our two virtual hosts we will be creating a file each that contains a server block of code with specific settings.

By default, Nginx contains one server block called default which we will be keeping as a reference to the default configurations but we wont be using it. 

We will begin by designing our first sites server block, which we will then copy over for our second site and make the necessary modifications. This procedure can then be used for any future sites you want to create for development purposes.
Create the First Server Block File
Our first server block we will be in a file that doesn’t currently exist so we will open its future location in Nano and when we save it it will be created for us.


sudo nano  /etc/nginx/sites-available/j34-dev1


Now make a copy of the code below with the standard highlight and copy combination and then in the Nano window right click and past it.

CODE

Note: Only one of our server blocks can have the default_server specification. This specifies which block should server a request if the server_name requested does not match any of the available server blocks.

We are eventually going to disable the default server block configuration, so we can place the default_server option in either this server block or in the one for our other site. I'm going to leave the default_server option enabled in this server block, but you can choose whichever is best for your situation.

Create the Second Server Block File
Now this one is easy we will be copying the last one and make a couple of small changes.

sudo cp  /etc/nginx/sites-available/j34-dev1 /etc/nginx/sites-available/j34-dev2

Now lets open our new file and makes some changes.

sudo nano  /etc/nginx/sites-available/j34-dev2

First remove the server next to this line for reasons I mentioned earlier.

listen 80;

update the server name to the new site name in our case it will become

server_name j34-dev2;

lastly change the error log location to reflect our new site location iso it will become

error_log /var/log/nginx/j34-dev2.error.log;

Feel free to research any of the settings I have chosen but keep in mind we are just going to use this server for development not for live sites.

Note: Each Nginx statement must end with a semi-colon (;), so check each of your lines if you are running into problems.


Enable your Server Blocks and Restart Nginx
You now have your server blocks created, we need to enable them. We can do this by creating symbolic links from these files to the sites-enabled directory, which Nginx reads from during startup.

We can create these links by typing:

sudo ln -s /etc/nginx/sites-available/j34-dev1 /etc/nginx/sites-enabled/
sudo ln -s /etc/nginx/sites-available/j34-dev2 /etc/nginx/sites-enabled/


These files are now in the enabled directory. However, the default server block file is also enabled currently and will conflict with our file that has the default_server parameter set.

We can disable the default server block file by simply removing the symbolic link. It will still be available for reference in the sites-available directory, but it won't be read by Nginx on startup.

sudo rm /etc/nginx/sites-enabled/default


Note: For any future sites you want to created just follow the same steps you used to create the second server block.

Now let restart our Nginx server and check for any issues.

sudo service nginx restart


Nginx should now be serving both of our new sites. Let have a look using your IP plus the name you have chosen for your websites.

http://192.168.1.104/j34-dev1/

Image



Install  PHP
# First lets do a little bit of maintenance to make sure our packages are upto date and our system is clean of unneeded fluff.

sudo sh -c "apt-get update;apt-get dist-upgrade;apt-get autoremove;apt-get autoclean"

# The packages required for PHP to work with Nginx is a little different to those when using PHP with Apache2. PHP runs as a FastCGI interface, so we need to install the PHP FPM package by typing the following command:

sudo apt-get install php5-fpm

Extra packages all at once

If you want to skip the details about each of aditional packages we will be installing and you would rather just install them all at once run the following command.

sudo apt-get install php5-fpm php-apc php5-curl php5-gd libssh2-php

Extra  packages in detail

If you want to learn a bit more about each package as you install them read on.

# To help speed things up we will also be installing Alternative PHP Cache. Its a free open-source opcode (operation code) caching plugin for PHP. With APC caching your PHP script executions can run more efficiently, by cutting down on dynamic PHP executions.

 sudo apt-get install php-apc

# We also want to install cURL and if you aren’t familiar with it it’s a library that lets you make HTTP requests in PHP.

sudo apt-get install php5-curl

#This package provides a module for handling graphics directly from PHP scripts. It supports the PNG, JPEG, XPM formats as well as Freetype/ttf fonts.

sudo apt-get php5-gd

#These bindings provide a method to utilise SSH connections with PHP 

sudo apt-get install libssh2-php
     
To improve the performance of PHP5-FPM, we need to install a PHP cacher:

sudo apt-get install php-apc

Note: If you ever need to clear the apc cache remember in our earlier guide we add a line to our PHP info page for just such an occasion. To use it just open the index.php file found in your root directory in the browser and thats it.

Configure PHP
If you aren't familiar with the php.ini file it contains configuration setting that affect your PHP installation. The tricky thing is to know which php.ini file should you edit because there can be multiple versions in multiple locations.

# In our particular case we will using the following file
/etc/php5/fpm/php.ini

# So lets update our PHP file with the following command.
sudo nano /etc/php5/fpm/php.ini

# now search for the following lines and update them accordingly

Tip: In the Nano editor you can use the ctrl w combination to search through the file.

# This sets the maximum amount of memory in bytes that a script is allowed to allocate

memory_limit = 128M
 
# The maximum size of an uploaded file.

upload_max_filesize = 64M
 
# Sets max size of post data allowed. This setting also affects file upload.

post_max_size = 64M

#Uncomment the following line (remove the semicolon) and make sure it is set to 0.

cgi.fix_pathinfo=0

Exit the editing interface by pressing ctrl+X, type y to confirm the changes and press enter to save the file path.

# Now to reload php and Ngnix 

sudo /etc/init.d/php5-fpm reload && sudo /etc/init.d/nginx reload

Text PHP
now lets test PHP by creating a PHP info page in our root directory

sudo nano /usr/share/nginx/www/index.php

and add the following lines

<?php 
// This will display PHP info.
phpinfo(); 
// This will reset the PHP APC cache.
opcache_reset();
?>

Exit the editing interface by pressing ctrl+X, type y to confirm the changes and press enter to save the file path. Then type your IP + /index.php into your browser.

http://192.168.1.104/index.php

You should see your new PHP info page and at the same time clear your apc cache which is good to have while you are developing.

Image

Install Mysql

# First lets do a little bit of maintenance to make sure our packages are upto date and our system is clean of unneeded fluff.

Note: this can take some time

sudo sh -c "apt-get update;apt-get dist-upgrade;apt-get autoremove;apt-get autoclean"

Next we’re going to install the MySQL server and client by typing:

sudo apt-get install mysql-server mysql-client

First you will be prompted to confirm that you want to install the server, client and their dependencies, chose Y.

image


Next you should  be prompted for a root password, choose a secure password, and keep it safe. You will need this later to create your databases and install Joomla.

image

Once you’ve confirmed your password the installation will finish and the services should start.

Image

Now we need to install one extra package, php5-mysql. The php5-mysql package allows connections to be made to MySQL Server through PHP.

sudo apt-get install php5-mysql

You will be prompted to confirm that you want to install php5-mysql and it’s dependencies, chose Y.

image

It will then continue install the relevant packages and it should at the end also restart php-fpm. 

image

Configure MySQL

The first thing we're going to do to optimize MySQL is replace the default my.cnf configuration file with one that is tuned for systems with less resources.

# lets make a backup first before moving any further

sudo mv /etc/mysql/my.cnf /etc/mysql/my.cnf.bak

#now lets copy over the my-small.cnf file from the examples directory.

sudo cp /usr/share/doc/mysql-server-5.5/examples/my-small.cnf /etc/mysql/my.cnf


Now the other thing we're going to do is set a size for MySQL's query cache. Basically, MySQL has the ability to cache query results in memory until the data behind them is changed, thus delivering the results faster. 

#It's up to you how big you want to make it, but as a default I'm just going to use 8 megabytes. So let open up our new cnf file.

sudo nano /etc/mysql/my.cnf

#Now navigate down to the [mysqld] section and place the follow line at the end.

query_cache_size = 8M

image


Exit the editing interface by pressing ctrl+X, type y to confirm the changes and press enter to save the file path. Now lets restart the MySQL server.

sudo service mysql restart

#If all went well you should see something like this.

image


Test MySQL

Because our server is only for development we are going to be using the root user to interact with our databases so lets test that now.

sudo mysql -uroot -hlocalhost -p

#enter the password you created earlier and you should be logged into MySQL.

IMAGE

Let create some databases for our new sites. I will be creating a new database for each of my sites using the same name as the site itself, this will make them easy to manage. I will be using the root user to create them.

#First log into MySql using the root user you create in the previous guide.

sudo mysql -uroot -hlocalhost -p

# Now create each database with the following command updating the name when appropriate.

CREATE DATABASE `j34-dev1`;

# when you have finished you can disconnect from MySql like this.

exit
