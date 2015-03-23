## Table of Contents
1.  [Installation Guides](#install)
    -   [Upload Package File](#upload)
    -   [Install From Directory](#directory)
    -   [Install From URL](#url)
    -   [Install From Web \[J3.+\]](#web)
2.  [Uninstallation Guides](#uninstall)
    -   [Uninstall](#uninstall-all)
3.  [Need More Help?](#more-help)

<div class="uk-alert">Note: CoalaWeb guides refer to a Joomla 3.+ installation but the steps are very similar for a Joomla 2.5.</div>

## <a class="doc-top" name="install"></a>Installation Guides

### <a name="upload"></a>Upload Package File

The first method of installing a CoalaWeb extension we are going to cover is the 
**Upload Package File** method. This is the most common method for installing Joomla 
extensions so it's a good place to start.

The first thing we need is a zipped up extension package ready to install so 
drop by the **Downloads** section of [CoalaWeb](http://coalaweb.com) and grab a copy of the 
extension you want to install. *\[Figure-1\]*

<span class="alert" markdown="1">Note: Before attempting to install a CoalaWeb extension make sure your system meets the minimum requirements.</div>

![Figure-1](http://cdn.coalaweb.com/images/docs/joomla-extensions/general/install/download-pack.png "Figure-1"){.coalaweb-docs}

Next log into the backend of your Joomla installation and open up the 
**Extension Manager** and then select the **Upload Package File** option.

It can be found in this location. *\[Figure-2\]*

    Extensions → Extension Manager → Upload Package File

![Figure-2](http://cdn.coalaweb.com/images/docs/joomla-extensions/general/install/upload-2.png "Figure-2"){.coalaweb-docs}

Then use the **Browse** button to find and select the package you downloaded in the first 
step. *\[Figure-3\]*

![Figure-3](http://cdn.coalaweb.com/images/docs/joomla-extensions/general/install/upload-3.png "Figure-3"){.coalaweb-docs}

Lastly select **Upload & Install** to start the process. The install script
used by CoalaWeb extensions will take care of installing all the related parts of 
the system such as **Modules** and **Plugins** and when it has 
finished you will receive conformation. *\[Figure-3\]*

<div class="uk-alert">Note: Installing an extension can take some time due to consisting of several smaller extensions so please be patient.</div>

![Figure-4](http://cdn.coalaweb.com/images/docs/joomla-extensions/general/install/install-confirm.png "Figure-4"){.coalaweb-docs}

### <a name="directory"></a>Install from Directory

The second method of installing a CoalaWeb extension we are going to cover is the 
**Install from Directory** method. This is a great way to install larger 
packages on system with limited resources. If your system timed out using the 
first method then this is the next logical step.

The first thing we need is an extension package ready to install so 
drop by the **Downloads** section of [CoalaWeb](http://coalaweb.com) and grab 
a copy of the extension you want to install. The difference with this method of 
installing an extension is that we need it unzipped so you may as well do it now. *\[Figure-1\]*

<div class="alert">Note: Before attempting to install a CoalaWeb extension make sure your system meets the minimum requirements.</div>

![Figure-1](http://cdn.coalaweb.com/images/docs/joomla-extensions/general/install/download-pack.png "Figure-1"){.coalaweb-docs}

Next we need to get the freshly downloaded package onto our server and into the
**tmp** directory so lets start by checking its location. Log into the backend 
of your Joomla installation and then head over to your **Server Settings** and check the
**Path to Temp Folder** as this is where we will be putting the package.

It can be found in this location. *\[Figure-2\]*

    System → Global Configuration → Server → Path to Temp Folder

![Figure-2](http://cdn.coalaweb.com/images/docs/joomla-extensions/general/install/directory-2.png "Figure-2"){.coalaweb-docs}

Now that we know where we want the package to go it's time to fire up your FTP client 
and navigate to the directory we just checked. Once we have found it upload the 
package we download in the first step into the **tmp** directory. *\[Figure-3\]*

<span class="alert" markdown="1">Note: Make sure the package is unzipped/extracted.</div>

![Figure-3](http://cdn.coalaweb.com/images/docs/joomla-extensions/general/install/directory-3.png "Figure-3"){.coalaweb-docs}

Now back to your Joomla administration area and open up the 
**Extension Manager** and then select the **Install from Directory** option.

It can be found in this location.

    Extensions → Extension Manager → Install from Directory

The **tmp** directory location should already be filled in for you and it should be the
same as the directory we check in a previous step. Next add the the package name 
to the end making sure it's exactly same as the folder you uploaded with FTP. *\[Figure-4\]*

![Figure-4](http://cdn.coalaweb.com/images/docs/joomla-extensions/general/install/directory-4.png "Figure-4"){.coalaweb-docs}

Lastly select **Install** to start the process. The install script
used by CoalaWeb extensions will take care of installing all the related parts of 
the system such as **Modules** and **Plugins** and when it has 
finished you will receive conformation. *\[Figure-5\]*

<div class="uk-alert">Note: Installing an extension can take some time due to consisting of several smaller extensions so please be patient.</div>

![Figure-5](http://cdn.coalaweb.com/images/docs/joomla-extensions/general/install/install-confirm.png "Figure-5"){.coalaweb-docs}

### <a name="url"></a>Install From URL

This option is a great way to install a CoalaWeb extension without needing to 
download it first.

<div class="alert">Note: Before attempting to install a CoalaWeb extension make sure your system meets the minimum requirements.</div>

<div class="alert">Note: To use this method you will need to be a registered and logged in user to access the link.</div>

Once you have logged in over at [CoalaWeb](http://coalaweb.com) proceed to the 
**Downloads** area the same as for the previous two methods of installing 
extensions and you will notice a new **Direct Link** option. *\[Figure-1\]*

![Figure-1](http://cdn.coalaweb.com/images/docs/joomla-extensions/general/install/url-1.png "Figure-1"){.coalaweb-docs}

Now copy this link and head back over to your Joomla administration area and open up the 
**Extension Manager** and then select the **Install from URL** option.

It can be found in this location.

    Extensions → Extension Manager → Install from URL

Next copy and paste the link from the previous step into the **Install URL** 
field. *\[Figure-2\]*

![Figure-2](http://cdn.coalaweb.com/images/docs/joomla-extensions/general/install/url-2.png "Figure-2"){.coalaweb-docs}

Lastly select **Install** to start the process. The install script
used by CoalaWeb extensions will take care of installing all the related parts of 
the system such as **Modules** and **Plugins** and when it has 
finished you will receive conformation. *\[Figure-3\]*

<div class="uk-alert" markdown="1">Note: Installing an extension can take some time due to consisting of several smaller extensions so please be patient.</div>

![Figure-3](http://cdn.coalaweb.com/images/docs/joomla-extensions/general/install/install-confirm.png "Figure-3"){.coalaweb-docs}

### <a name="web"></a>Install from Web J3.+

The last way to install a CoalaWeb extension we are going to cover is the new Joomla 3.+
**Install from Web** option which is a quick and easy way to try out our **Core**
extensions.

<div class="alert">Note: Before attempting to install a CoalaWeb extension make sure your system meets the minimum requirements.</div>

First log into the backend of your Joomla installation and open up the 
**Extension Manager** then select the **Install from Web** option.

It can be found in this location.

    Extensions → Extension Manager → Install from Web

Next in the **Search** box type **coalaweb** and click the magnifying glass. 
You should now see a list of our extensions. *\[Figure-1\]*

![Figure-1](http://cdn.coalaweb.com/images/docs/joomla-extensions/general/install/web-1.png "Figure-1"){.coalaweb-docs}

For this example we will install the **CoalaWeb Social Links** extension so 
click the title of the extension you want to install. You should now see a 
description page along with some links included an **Install** link. *\[Figure-2\]*

![Figure-2](http://cdn.coalaweb.com/images/docs/joomla-extensions/general/install/web-2.png "Figure-2"){.coalaweb-docs}

Next click **Install** and you will be taken to a confirmation page with basic
details about the extension and its download link. *\[Figure-3\]*

![Figure-3](http://cdn.coalaweb.com/images/docs/joomla-extensions/general/install/web-3.png "Figure-3"){.coalaweb-docs}

If you are happy select **Install** again to start the process. The install script
used by CoalaWeb extensions will take care of installing all the related parts of 
the system such as **Modules** and **Plugins** and when it has 
finished you will receive conformation. *\[Figure-4\]*

<div class="uk-alert">Note: Installing an extension can take some time due to consisting of several smaller extensions so please be patient.</div>

![Figure-4](http://cdn.coalaweb.com/images/docs/joomla-extensions/general/install/install-confirm.png "Figure-4"){.coalaweb-docs}

## <a name="uninstall"></a>Uninstallation Guides

### <a name="uninstall-all"></a>Uninstall

Coalaweb extensions come with an install script that takes care of installing all 
the parts system in one go such as a components, modules and plugins. The same 
script also does the work of uninstalling all the parts of the system as well 
but the trick is to uninstall the associated component as it contains the 
install/uninstall script.

First log into the backend of your Joomla installation and open up the 
**Extension Manager** then select **Manage** from the menu. *\[Figure-1\]*

It can be found in this location.

    Extensions → Extension Manager → Manage

![Figure-1](http://cdn.coalaweb.com/images/docs/joomla-extensions/general/install/uninstall-all-1.png "Figure-1"){.coalaweb-docs}

Next to make sure we only have components listed change the filter **Type** to 
**Components** now you should only have components listed to the right. *\[Figure-2\]*

![Figure-2](http://cdn.coalaweb.com/images/docs/joomla-extensions/general/install/uninstall-all-2.png "Figure-2"){.coalaweb-docs}

Next to filter down the extensions even more lets use the search box and search 
for **coalaweb** In the case of this guide we will be uninstalling the 
CoalaWeb Social Links extension. *\[Figure-3\]*

![Figure-3](http://cdn.coalaweb.com/images/docs/joomla-extensions/general/install/uninstall-all-3.png "Figure-3"){.coalaweb-docs}

Now select it from the list and click **Uninstall** from the top menu. The uninstall script
used by CoalaWeb extensions will take care of uninstalling all the related parts of 
the system such as **Modules** and **Plugins** and when it has 
finished you will receive conformation. *\[Figure-4\]*

<div class="uk-alert">Note: Uninstalling an extension can take some time due to having to uninstall several smaller extensions at the same time so please be patient.</div>

![Figure-4](http://cdn.coalaweb.com/images/docs/joomla-extensions/general/install/uninstall-all-4.png "Figure-4"){.coalaweb-docs}

Now if you have other CoalaWeb extension installed on your system than thats it
you have finished. If this was the only CoalaWeb extension you had installed 
then you have one last step. A system plugin called **CW Gears** is installed 
with every CoalaWeb extension and acts a small framework and because every 
CoalaWeb extension needs it it isn't automatically uninstalled.

Let make it easy to find by doing some filtering, select **Plugin** from the 
**Filter** menu and then type **CW Gears** in the search field. *\[Figure-5\]*

![Figure-5](http://cdn.coalaweb.com/images/docs/joomla-extensions/general/install/uninstall-all-5.png "Figure-5"){.coalaweb-docs}

Select the **CW Gears** plugin and then click **Uninstall** from the top menu. When it 
has finished you will receive confirmation and you are done. *\[Figure-6\]*

![Figure-6](http://cdn.coalaweb.com/images/docs/joomla-extensions/general/install/uninstall-all-6.png "Figure-6"){.coalaweb-docs}

## <a name="more-help"></a>Need More Help

<div class="uk-alert">Do you have a question that wasn't covered by the GUIDE? Then it's time to drop by the [Forum](http://coalaweb.com/forum/index)</div>