## Table of Contents
1.  [Overview](#overview)
2.  [Component Guide](#component-guide)
    -   [Control Panel](#control-panel)
    -   [Visitors](#visitors)
    -   [IP Categories](#ip-cats)
    -   [Known IPs](#knownips)
        - [1. IP Formats](#ki-ips)
        - [2. Scenarios](#ki-scenarios)
    -   [GEO Location](#geo)
        - [1. Install](#geo-install)
        - [2. Easy Install](#geo-easy)
        - [3. Manual Install](#geo-manual-core)
        - [4. Manual Install \[Pro\]](#geo-manual-pro)
    -   [Charts \[Pro\]](#com-charts)
    -   [CSV Report](#export-csv)
    -   [Purge](#com-purge)
    -   [Optimize \[Pro\]](#com-optimize)
    -   [Add Robots \[Pro\]](#com-robots)
    -   [Help](#help)
    -   [Options](#options)
3.  [Traffic \[M\]](#module)
    -   [General](#mod-general)
    -   [Layout](#mod-layout)
    -   [Visitor](#mod-visitor)
    -   [Who is Online](#mod-who)
    -   [Advanced](#mod-advanced)
4.  [Plugins](#plg)
    -   [System Plugin - Count](#plg-count)
    -   [System Plugin - Clean](#plg-clean)
    -   [System Plugin - Online](#plg-online)
5.  [Need More Help?](#more-help)

## <a class="doc-top"  name="overview"></a>Overview

**CoalaWeb Traffic** is a Joomla extension designed to keep track of the visitors to your site. You can choose to display the modules and let visitors see and be amazed by your traffic or unpublish the module and view your website statistics in the **Admin** area.

<div class="uk-alert">When installing all the parts of the system will be installed at the same time making installing, upgrading and uninstalling a breeze.</div>

## <a name="component-guide"></a>Component

### <a name="control-panel"></a>Control Panel

The **Control Panel** as seen below it is designed to be an easy starting point, think of it as the components head quarters. While carrying out tasks you can easily jump from the **Control Panel** to the different sections and then return before moving onto the next one. *\[Figure-1\]*

![Figure-1](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-cpanel.png "Figure-1"){.coalaweb-docs}

### <a name="visitors"></a>Visitors

![Figure-2](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-visitors.png "Figure-2"){.coalaweb-docs}

The Visitors section is where all the visitors to your site are listed. The visitors are displayed with the following information.

-   Their IP address (unless not stored RAW)
-   Browser Type
-   Browser Version
-   Platform (Operating System)
-   Referer Link
-   The date they visited
-   The time they visited
-   Name assignment (optional)
-   Their Location (Only with the Geo Database Installed)

Both **Core** and **Pro** users have sort and search options. To sort the visitor information you can click the column **Heading** or use the **Select list** in the top right. The avaliable sorting options are:

-   IP
-   Browser
-   Platform
-   Date
-   Country
-   ID

You also have a search box where you can choose to enter an **IP** or **Date** to search for specific visitor information. *\[Figure-2a\]*

![Figure-2a](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-visitors-1.png "Figure-2a"){.coalaweb-docs}

**Pro** subscribers also get **Filter** options which can be used by clicking the **Search Tools** button at the top and include **Browser**, **Platform** and **Country** select lists. *\[Figure-2b\]*

![Figure-2b](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-visitors-2.png "Figure-2b"){.coalaweb-docs}

### <a name="ip-cats"></a>IP Categories

![Figure-3](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-ip-cats.png "Figure-3"){.coalaweb-docs}

To make it easier to organize your **Know IPs** you can create categories to associated them with. For example you could create a category called **Robots** and then add all the known robots in your **Knownips** list to this category. *\[Figure-3a\]*

![Figure-3a](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-ip-cats-1.png "Figure-3a"){.coalaweb-docs}

### <a name="knownips"></a>Known IPs

![Figure-4](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-knownips.png "Figure-4"){.coalaweb-docs}

The next section is the **Known IPs** section which contains some powerful tools for controlling what is counted by **Traffic**.  *\[Figure-4a\]*.

![Figure-4a](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-knownips-1.png "Figure-4a"){.coalaweb-docs}

### <a name="ki-ips"></a>IP Formats

![Figure-3](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-knownips-2.png "Figure-3"){.coalaweb-docs}

When adding IPs to a Known IP entry you have several options, you can specify an IP or IP range in the following formats:

-   Single IP - 192.168.1.1
-   Simple IP Range - 192.168.1.1-192.168.1.255
-   Implied IP Range - 192.168.1.

### <a name="ki-scenarios"></a>Scenarios

**Your Own IP:**

If you just want to keep an eye on your own IP for example you could create a new entry give it a **Name** and **Description** add your **IP** and leave **Count** to yes. Now in the **Visitors** view you can see your visits easily by look down the **IP Owner** column. *\[Figure-3\]*.

**Block by IP:**

If you want to stop an IP from being counted by **Traffic** create a new entry give it a **Name** and **Description** add the **IP** and set **Count** to **No**. Now that particular IP will not appear in the visitors list as it is not counted by the system any more.

**Block by Name:**

If you want to stop a robot from being counted by **Traffic** based on it's **Name** create a new entry give it a **Name** and **Description** add the **Robot Name** and set **Count** to **No**. Now that particular robot will not appear in the visitors list as it is not counted by the system any more.

<div class="uk-alert" >Note: The most reliable way to identify visitors is by their IP the name information comes from their <em>user agent string</em> which isn't always supplied.</div>

### <a name="geo"></a>GEO Location

CoalaWeb Traffic gives you the option to identify your visitors **Countries** and **Cities** of origin based on their IP addresses. *\[Figure-5\]*.

![Figure-5](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-geo-1.png "Figure-5"){.coalaweb-docs}

#### How Geo Location Works

CoalaWeb Traffic can work in conjunction with **MaxMind's** Geo databases to help determine location information about your visitors. The **Core** version of CoalaWeb Traffic uses the **(Legacy) GeoLite City** database while **Pro** subscribers get the advantage of using the current **GeoLite2 City** database with extend features. The databases are updated very frequently, about once every month. Why so often? IP assignments to countries change all the time in fact by the time we release our extension, the database file is most likely already slightly out of date.

#### What Will This Affect

This could cause some IP addresses to be identified as coming from the wrong location. Updating the file regularly will give you much better country and city accuracy. [MaxMind](http://dev.maxmind.com/geoip/geolite) claims an accuracy of 99.5% for its free Geo databases so please bear in mind that this means that some IP addresses might be reported wrongly.

#### Do I Have To Install It?

**No you do not.** The system will continue to count and store your website traffic with out the database installed the only difference is that you won't see *Country* or *City* information associated with their IP addresses.

<div class="uk-alert">Note: It's a good idea to inform visitors in your privacy policy or TOS that you are collecting their information.</div>

#### <a name="geo-install"></a>Installing the Geo Database

If you don’t have the **GeoLiteCity** database installed you will receive a notice message. To take advantage of CoalaWeb Traffics inbuilt ability to tell you a visitors country and sometimes
their city follow the steps below. *\[Figure-5a\]*.

![Figure-5a](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-geo-2.png "Figure-5a"){.coalaweb-docs}

To make it easier to know if you will need to upload the database manually I have added a **Upload Minimum Requirements** check list that will display in the Geo Location view. *\[Figure-5b\]*.

![Figure-5b](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-geo-3.png "Figure-5b"){.coalaweb-docs}

<div class="uk-alert">If your system doesn't meet the minimum requirements but its close I recommend trying the easy way first before moving on to the manual method.</div>
 
#### <a name="geo-easy"></a>Easy Install

First click the **Upload Geo Database** blue button this will retrieve the latest version of the database from the **Maximind** website and upload it to your website's **tmp** directory. *\[Figure-5c\]*.

![Figure-5c](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-geo-4.png "Figure-5c"){.coalaweb-docs}

If everything went according to plan you will receive a conformation message that it uploaded correctly. *\[Figure-5d\]*.

![Figure-5d](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-geo-5.png "Figure-5d"){.coalaweb-docs}

The next step is to **Unzip** the file to the CoalaWeb Traffic geoip directory where it can be accessed and used to determine your visitors locations. If the database uploaded correctly in the last step you will now have a **Unzip** icon in the top tool bar, click this to start the unzip process. *\[Figure-5e\]*.

![Figure-5e](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-geo-6.png "Figure-5e"){.coalaweb-docs}

Once again if everything goes according to plan you receive a conformation message that the file was unzipped correctly and also the message at the top of the page will turn green with today's date. *\[Figure-5f and Figure-5l\]*.

![Figure-5f](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-geo-7.png "Figure-5f"){.coalaweb-docs}

![Figure-5l](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-geo-13.png "Figure-5l"){.coalaweb-docs}

Now CoalaWeb Traffic will automatically add country and city information to your visitor records as they are collected. To keep the location information as accurate as possible just carry out this procedure at regular intervals.

<div class="uk-alert">Note: Please be patient when <em>Uploading</em> and <em>Unzipping</em> the database it may take some time due to the size of the file.</div>

#### <a name="geo-manual-core"></a>Manual Install

If you re using the **Core** version of **Traffic** and you couldn't install the database the easy way no problem lets just do it the manual way by following these steps.

<div class="uk-alert">Note: To avoid issues please follow these steps exactly as they are written.</div>

Download the latest MaxMind **GeoLiteCity** database [HERE](http://geolite.maxmind.com/download/geoip/database/GeoLiteCity.dat.gz). *\[Figure-5g\]*.

![Figure-5g](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-geo-8.png "Figure-5g"){.coalaweb-docs}

Now that you have the database downloaded the next step is to extract it. Once it has completed the extraction process you will have a file named **GeoLiteCity.dat** *\[Figure-5i\]*.

![Figure-5i](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-geo-10.png "Figure-5i"){.coalaweb-docs}

The next step is convert the name to lowercase **geolitecity.dat**. *\[Figure-5j\]*.

![Figure-5j](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-geo-11.png "Figure-5j"){.coalaweb-docs}

The last step is to upload your newly renamed database file to the following location:

    administrator/components/com_coalawebtraffic/assets/geoip

The database file should have 644 permissions. *\[Figure-5k\]*.

![Figure-5k](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-geo-12.png "Figure-5k"){.coalaweb-docs}

Now if everything went according to plan you should now start to see **Country and City** data in the **Visitors** view.

#### <a name="geo-manual-pro"></a>Manual Install \[Pro\]

If you re using the **Pro** version of **Traffic** and you  couldn't install the database the easy way no problem lets just do it the manual way by following these steps.

<div class="uk-alert">Note: To avoid issues please follow these steps exactly as they are written.</div>

Download the latest MaxMind **GeoLite2 City** database [HERE](http://geolite.maxmind.com/download/geoip/database/GeoLite2-City.mmdb.gz). *\[Figure-5g-a\]*.

![Figure-5g-a](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-geo-8a.png "Figure-5g-a"){.coalaweb-docs}

Now that you have the database downloaded the next step is to extract it. Once it has completed the extraction process you will have a file named **GeoLite2-City.mmdb** *\[Figure-5i-a\]*.

![Figure-5i-a](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-geo-10a.png "Figure-5i-a"){.coalaweb-docs}

The next step is convert the name to lowercase **geolite2-city.mmdb**. *\[Figure-5j-a\]*.

![Figure-5j-a](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-geo-11a.png "Figure-5j-a"){.coalaweb-docs}

The last step is to upload your newly renamed database file to the following location:

    administrator/components/com_coalawebtraffic/assets/geoip/v2

The database file should have 644 permissions. *\[Figure-5k-a\]*.

![Figure-5k-a](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-geo-12a.png "Figure-5k-a"){.coalaweb-docs}

Now if everything went according to plan you should now start to see **Country and City** data in the **Visitors** view.

### <a name="com-charts"></a>Charts \[Pro\]

Pro subscribers also get access to a series of **Charts** which allow you to quickly see your visitor data grouped in the following ways.

#### Visitors

A quick summary of your visitors displayed in a graph based on quantity and date accompanied by a summary table. *\[Figure-14\]*.

![Figure-14](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-chart-1.png "Figure-14"){.coalaweb-docs}

#### Countries

A color coded map visual representing your visitors and their countries accompanied by a summary table. *\[Figure-14a\]*.

![Figure-14a](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-chart-2.png "Figure-14a"){.coalaweb-docs}

#### Cities

A color coded pie chart representing your visitors and their cities accompanied by a summary table. *\[Figure-14b\]*.

![Figure-14b](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-chart-3.png "Figure-14b"){.coalaweb-docs}

#### Browsers

A color coded pie chart representing your visitors and their browsers accompanied by a summary table. *\[Figure-14c\]*.

![Figure-14c](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-chart-4.png "Figure-14c"){.coalaweb-docs}

#### Platforms

A color coded pie chart representing your visitors and their platforms accompanied by a summary table. *\[Figure-14d\]*.

![Figure-14d](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-chart-5.png "Figure-14d"){.coalaweb-docs}

### <a name="export-csv"></a>CSV Report

If you want to export the visitors currently stored in your database start by clicking the **CSV Report** button in the **Control Panel**.

![Figure-6](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-export-1.png "Figure-6"){.coalaweb-docs}

You should get a pop up that similar to the image below if not make sure it's not being blocked by something such as your browser settings. *\[Figure-6c\]*

![Figure-6c](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-export-4.png "Figure-6c"){.coalaweb-docs}

Next save the file to your local computer and then open it with your application of choice. In this example I will be using **LibreOffice** but the procedure will be similar with other applications. First I have to import it before I can work with the data so after a double click I'm confronted with the window below. *\[Figure-6d\]*

![Figure-6d](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-export-5.png "Figure-6d"){.coalaweb-docs}

I have chosen to import it with the default settings which results in the data being laid out in a sheet.  *\[Figure-6e\]*

![Figure-6e](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-export-6.png "Figure-6e"){.coalaweb-docs}

You can now format, filter and save the data as you wish.

### <a name="com-purge"></a>Purge

![Figure-32a](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-purge1.png "Figure-32a"){.coalaweb-docs}

The **Purge** button will delete all of the traffic records current stored in the Traffic database tables. To make sure you haven't accidentally press it you will get a popup asking you to confirm your choice. *\[Figure-32b\]*

![Figure-32b](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-purge2.png "Figure-32b"){.coalaweb-docs}

After it has completed you get a confirmation message or an error message if it was unable to carry out the task. *\[Figure-32c\]*

![Figure-32c](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-purge3.png "Figure-32c"){.coalaweb-docs}

### <a name="com-optimize"></a>Optimize and Repair \[Pro\]

![Figure-33a](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-optimize1.png "Figure-33a"){.coalaweb-docs}

Pro subscribers also get an **Optimize** button which will attempt to repair and optimize all the Traffic database tables. To make sure you haven't accidentally press it you will get a popup asking you to confirm your choice. *\[Figure-33b\]*

![Figure-33b](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-optimize2.png "Figure-33b"){.coalaweb-docs}

After it has completed you get a confirmation message or an error message if it was unable to carry out the task. *\[Figure-32c\]*

![Figure-33c](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-optimize3.png "Figure-33c"){.coalaweb-docs}

### <a name="com-robots"></a>Add Robots \[Pro\]

![Figure-32a](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-robots-1.png "Figure-32a"){.coalaweb-docs}

The **Add Robots** button allows **Pro** subscribers to auto populate the **Known IP** list with a list of known **Robots** instantly stopping them from being counted. To make sure you haven't accidentally press it you will get a popup asking you to confirm your choice. *\[Figure-32b\]*

![Figure-32b](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-robots-2.png "Figure-32b"){.coalaweb-docs}

After it has completed you get a confirmation message or an error message if it was unable to carry out the task. *\[Figure-32c\]*

![Figure-32c](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-robots-3.png "Figure-32c"){.coalaweb-docs}

<div class="uk-alert">The <em>Add Robots</em> system will compare the current list to what you have stored and add any new robots as needed so it's a good idea to run it after each update.</div>

### <a name="help"></a>Inbuilt Help

In the control panel or the tool menu you have a help icon that when clicked will open a pop up wrapper of this specific guide. This gives you an easy way of checking the functionality of a particular item without leaving the control panel. *\[Figure-7\]*

![Figure-7](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-help.png "Figure-7"){.coalaweb-docs}

### <a name="options"></a>Extension Options

![Figure-8](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-options.png "Figure-8"){.coalaweb-docs}

In the control panel or the tool menu you have a **Options** icon that when clicked will open a series of extension options.

#### General Options

The first option in this section is the **Locktime** this is the amount of time that must pass before a particular IP will be counted again. It is measured in minutes and 1440 (Full day) is the default. *\[Figure-8\]*

The next option is **Week Start** which allows you to choose which day you want the calculations for the **Weeks** visitors to start from. This only affects the week count in the front end module and the back end statistics area of the control panel. *\[Figure-8\]*

The last option in this section is the **Preset Counter** this number will be added to the current **Total** so its good for when you move a site or to bump up the visitors. This only affects the total count in the front end module and the back end statistics area of the control panel. *\[Figure-8a\]*

![Figure-8a](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-options-1.png "Figure-8a"){.coalaweb-docs}

#### Storage \[Pro\]

The first option in th is section is to turn on or off the storing of IPs in **Raw** format otherwise they will only be stored in an unreadable hash format. If you choose no for this option then in the visitors view **Not Stored Raw!** will be displayed in the IP column and every visitor recorded after that will not have its IP stored in raw format in the database. *\[Figure-8e\]*

The second option is to turn on or off the storing of Geo location information. Even if you are not storing IPs in their raw format you can still have Geo information recorded as long as you have uploaded a Geo database. *\[Figure-8e\]*

![Figure-8e](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-options-6.png "Figure-8e"){.coalaweb-docs}

#### Robots \[Pro\]

The option in this section will use Joomla's JApplicationWebClient class to block a few well known robots from being counted. This will only detects basic robots if you wish to block additional robots use the KnownIPs list. *\[Figure-8f\]*

![Figure-8f](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-options-7.png "Figure-8f"){.coalaweb-docs}

#### Cleanup

In this section you can control the automatic clean up of the database to stop the tables filling up with data. I recommend having this set to on and the second option of how many **Records to Keep** will depend on your circumstances. *\[Figure-8b\]*

![Figure-8b](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-options-2.png "Figure-8b"){.coalaweb-docs}

#### Project Honeypot

Project Honeypot is a collective effort to detect spammers, email harversters and crackers. Its HTTP:BL service allows participants to query the IP addresses of their visitors and figure out if it is a malicious user behind it. If you enable this feature, CoalaWeb Traffic will check the IP address of each visitor and, if it is a malicious user, it will not count them. *\[Figure-8b\]*

![Figure-8b](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-options-3.png "Figure-8b"){.coalaweb-docs}

<div class="uk-alert">Note: CoalaWeb Traffic does not block visitors from your site only from being counted by the Traffic system.</div>

**Use Project Honeypot**

-   This option is an easy one it turns the feature on and off

**API key**

-   Enter your HTTP:BL key. You can sign up for Project Honeypot and get your key at http://www.projecthoneypot.org/httpbl_configure.php.

**Block suspicious**

-   Sometimes Project Honeypot is not sure if an IP belongs to a spammer or someone who made a couple of bad decisions while surfing the web. In this case the IP is marked as "suspicious". The default behaviour is to not block these IPs. 

**Block Search Engines**

-   If you don't want search engines being counted as visitors to your site you can turn this on. This does not guarantee that all search engines won't be counted but it's a good start. 

**Minimum Threat (0-255, default 25)**

-   Project Honeypot uses a logarithmic "threat rating" to rank the possibility of a specific IP being a spammer. This options defines the minimum threat level an IP must have before it's blocked. A value of 25 means that this IP has submitted 100 spam messages on Project Honeypot's spam catching honeypots and is usually a safe indication that it belongs to a spammer. Do note that the rating is logarithmic. A value of 50 means 1,000 spam messages and a value of 75 means one million spam messages. Do not set it to values over 50, as you will most likely never block any spammer at all.

**Maximum Age**

-   Project Honeypot reports when was the last time this IP was caught sending spam messages. The older this is (the higher the age is), the less likely is that this IP is still used by a spammer. You can chose here what will be the maximum reported age that will be blocked. The default value of 30 means that IPs which have submitted a spam message in the last 30 days will be blocked.

#### Obsolete

The options in this section are obsolete and have been included to allow users an opportunity to transfer them to the new system. *\[Figure-8c\]*

![Figure-8c](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-options-4.png "Figure-8c"){.coalaweb-docs}

#### Permissions

Lastly you have the permissions used to control access tothe CoalaWeb Traffic component. *\[Figure-8d\]*

![Figure-8d](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-options-5.png "Figure-8d"){.coalaweb-docs}


# <a name="module"></a>CoalaWeb Traffic Module

The CoalaWeb Traffic module has a huge list of options so we have broken them up into several sections which are explained in detail below.

<div class="uk-alert">If you have a multilingual website please leave text fields found through out the module configuration blank and instead use language files to control the text.</div>

### <a name="mod-general"></a>General Display Options

To make it easy to explain I have broken this section up into two parts.

**Part 1 Digital Counter**

First you can choose if you want to display the digital counter section at all 
maybe you only want to display individual counters. Next you can choose how many 
digits you want to be displayed. The last option in this section is to choose a theme
for your digital counter. *\[Figure-9\]*

![Figure-9](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-mod-general-1.png "Figure-9"){.coalaweb-docs}

**Part 2 Individual Counters**

First you can choose if you want to display the individual counters section at all 
maybe you only want to display a digital counter. The next option is to choose a 
theme, this will affect which icons are displayed along side the 
individual counters or you can choose to have no icons. 

Next you have the ability to turn on or off the display for
today, yesterday, this week, this month and total it's up to you which ones you
want to display. Under each of these options is a text box here you can
assign a word to be displayed next to the item but if your site is
multilingual leave these blank and use the language files to control
what is displayed. *\[Figure-9a\]*

![Figure-9a](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-mod-general-2.png "Figure-9a"){.coalaweb-docs}

### <a name="mod-layout"></a>Module Layout Options

The first two options control the width of the counter section and the overall
module width.

The next option is the module layout you have three options to choose from.

-   **Default** - The vertical layout allows both the counters and visitor info.
-   **Horizontal** - The horizontal layout only allows counters.
-   **Compact** - The compact layout only displays the horizontal text and the total counter.

The next option is the horizontal text this will display to the left of
both the horizontal and compact layouts. The last option is the
separator this will display between items in both the horizontal and
compact layouts. *\[Figure-10\]*

![Figure-10](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-mod-layout-1.png "Figure-10"){.coalaweb-docs}

### <a name="mod-visitor"></a>Visitor Display Options

This section controls what information about the visitor will be displayed within 
the **Traffic** module. 

To make it easier to explain I have broken this section into two parts.

**Part 1**

First you can choose if you want to display the visitor information section at all.
Next are the **Title** configuration options, you can to choose to display one 
including the title text, it's format and it's alignment.The next option turns 
on or off a horizontal line to separate the counter items from the visitor 
information. *\[Figure-11\]*

![Figure-11](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-mod-visitor-1.png "Figure-11"){.coalaweb-docs}

**Part 2**

In this section you have the option to turn on or off the following items as well
as choosing their label text.  *\[Figure-11a\]*

-   IP
-   Browser
-   Operating System

![Figure-11a](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-mod-visitor-2.png "Figure-11a"){.coalaweb-docs}

### <a name="mod-who"></a>Who is Online Options

Due to the flaws in the Joomla method of tell who is online I have created my own
that uses cookies and a database table to keep track of who is online. The data 
is then retrieved and displayed in this section of the module.

First you can choose if you want to display the who is online section at all.
Next are the **Title** configuration options, you can to choose to display one 
including the title text, subtitle text, it's format and it's alignment.The next option turns 
on or off a horizontal line to separate the counter items from the visitor 
information. *\[Figure-12\]*

![Figure-12](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-mod-who-1.png "Figure-12"){.coalaweb-docs}

### <a name="mod-advanced"></a>Advanced Options

The CoalaWeb Traffic module also has a few of what I consider
**Advanced Options** such as the option to assign a **Unique Module ID**
to stop conflicts, a **Module Class Suffix** or whether to use **Cache**
including the **Cache Time**. This next option allows you to display the 
**Date and Time** at the bottom of the module as well as choosing its **Format**. 

The last option is whether to display a **Link Back to CoalaWeb** which is always appreciated but its up to you
plus you can choose what text to display next to the link. *Note: If
your site is multilingual leave blank and use the language files. *\[Figure-13\]*

![Figure-13](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-mod-advanced-1.png "Figure-13"){.coalaweb-docs}

# <a name="plg"></a>Plugins

There are several plugins crucial to the proper functioning of the CoalaWeb 
Traffic system. They are explain in detail below.

## <a name="plg-count"></a>System Plugin - Count

This plugin is crucial to functionality of the system it quietly counts
the visits to your site and then records them in the database. It allows
you to count the traffic to your site even with the module unpublished
and also ensures all traffic is record regardless of the part of the
site that they visit.

This plugin also takes care of blocking visitors from being counted based on your 
setting in the CoalaWeb Traffic component.

<div class="uk-alert">Note: To ensure proper functionality of CoalaWeb Traffic please make sure this plugin is installed and publish.</div>

## <a name="plg-clean"></a>System Plugin - Clean

This plugin carries out the automatic database clean up but only if you
have it turned on in the **Component Options**. It will run in the
background keeping the current data but delete out the old entries and
then add them to a running total. It is recommended to turn this feature
on.

<div class="uk-alert">Have you chosen automatic database clean up? Then this plugin needs to be installed and published.</div>

## <a name="plg-online"></a>System Plugin - Online

This plugin will count and then supply the information so the **Traffic** 
module can display the currently online visitors. It uses it own database table 
along with cookies to keep track of visitors.

<div class="uk-alert">Have you chosen to display <em>Who is Online?</em> Then this plugin needs to be installed and published.</div>

## <a name="more-help"></a>Need More Help

<div class="uk-alert">Do you have a question that wasn't covered by this GUIDE? Try the <a href="http://coalaweb.com/support/documentation/category/traffic" target="_self">FAQ</a></div>

<div class="uk-alert">Do you have a question that wasn't covered by this GUIDE or the FAQ? Then it's time to drop by the <a href="http://coalaweb.com/forum/index" target="_self">Forum</a></div>