There are lots of reason why you might want to disable a plugin from not needing it anymore to stopping a plugin from producing a website crashing error. In some cases just a missing variable that a plugin is looking for is enough to halt an entire website until its rectified and in these cases the quickest fix is to disable the offending plugin.

### 1. Plugin Manager

The first way  we are going to discuss is the method you will use in most cases and it involves using the **Plugin Manager**. *[Figure-1]*

![Figure-1](images/docs/joomla/extensions/general/disable-plugin/opt1-1.png "Figure-1"){.coalaweb-docs}


The hardest part of this method is finding the plugin you're looking for, in our example we are going to be disabling the **System - CW Gears** plugin. The easiest way to find it would be to type **Gears** in the search box. *[Figure-1a]*

![Figure-1a](images/docs/joomla/extensions/general/disable-plugin/opt1-2.png "Figure-1a"){.coalaweb-docs}

What If you aren’t exactly sure what the plugin is called? To start with you can use some of the filters to reduce the amount of plugins you will have to look through. For example if you are trying to disable a plugin we can assume it is currently enabled so setting the Select Status filter to Enabled would help. *[Figure-1b]*

![Figure-1b](images/docs/joomla/extensions/general/disable-plugin/opt1-3.png "Figure-1b"){.coalaweb-docs}

Once you have found the plugin you are looking for its just a matter of clicking the Status icon to disable or enable it. *[Figure-1c]*

![Figure-1c](images/docs/joomla/extensions/general/disable-plugin/opt1-4.png "Figure-1c"){.coalaweb-docs}

If you want to disable multiple plugins at the same time you use the check-boxes next to each of them and then use the Disable or Enable button from the top menu. *[Figure-1d]*

![Figure-1d](images/docs/joomla/extensions/general/disable-plugin/opt1-5.png "Figure-1d"){.coalaweb-docs}

### 2. Editing Extension Files

If a plugin is for example stopping you from accessing the Plugin Manager your next logical step would be disabling it via a file manager or FTP client. With this method again it is dependent on knowing the name of the plugin you are trying to disable including what plugin group it belongs to as it will be stored in directory of the same name. If your website is inaccessible then there is a good chance the plugin to blame is from one of these three groups.

plugins->authentication
plugins->content
plugins->system

For this example I will be access the root of my website and then the plugins directory via FTP and it will look something like the image below. image

image

Once again we will be using the System - CW Gears plugin for this example so we will need to drill down through the following directories. Image

plugins -> system -> cwgears

image

The main two plugin files will be the php and xml files with the same name as the plugin’s directory so in this example.

cwgears.php
cwgears.xml

To disable it we want to rename or remove the php file. In my opinion its better to rename it and once you get access to your site again you can always uninstall it through the Plugin Manager. For this example we will rename it to cwgears.php-off. image

image

Now you should be able to gain access again to your website and take the appropriate action.

### 3. Editing Database Entry

This is the option that will require you to have the most access to your website, knowledge and inherent risk because we will be editing a database table so it should be your last resort. The second option covered in this guide should be all you ever need but if not read on.

In this example we will be using phpMyAdmin to access the database as it is the most widely used tool and normally comes package with your administration portal such as Cpanel. If you are using another tool to administer your database the principals are the same.

Once you have logged into to phpMyAdmin select the database associated with your website from the left you should be looking a list of all your website tables and the one we are interested in is the extensions table so once you have found it click it. image

image

In the next window you will see a list of all the extension contained on your website including the components, modules and plugins so to get to the one we are looking for lets use the Search tab from the top. image

image

In the next window you have several ways to filter the extension I prefer to use the Element field as its the same as the directory the plugin is stored in but you could use type (plugin) and folder(system) for example to help find the one you are looking for. When you are ready click the Go button in the bottom right to start the search which in my case returned the plugin I was looking for with the field I used to search highlighted. You may also notice that it has a 1 in the Enabled column telling us that it is currently enabled.  Image

image

Now to disable the plugin in question just click the inline edit button to the left which will allow us to make quick changes to the table. image

image

In the next window look for the column titled enabled and change the 1 to a 0 and click save from the left menu. Thats it the plugin is now disabled and you should have gained access again to your website. If you need to disable more plugins just repeats the steps.

Tips
If you see an error message take note of the file that is causing the problem as there is a good chnace it will tell you which plugin is to blame. image

image














