## Table of Contents
1.  [Component Guide](#component-guide)
    -   [Control Panel](#control-panel)
    -   [Visitors](#visitors)
    -   [IP Categories](#ip-cats)
    -   [Known IPs](#knownips)
        - [1. IP Formats](#ki-ips)
        - [2. Scenarios](#ki-scenarios)
    -   [GEO Location](#geo)
        - [1. Install](#geo-install)
        - [2. Easy Install](#geo-easy)
        - [3. Manual Install](#geo-manual)
    -   [CSV Export Option](#export-csv)
    -   [Inbuilt Help](#help)
    -   [Extension Options](#options)
2.  [Module Guide](#module)
    -   [General Options](#mod-general)
    -   [Layout Options](#mod-layout)
    -   [Visitor Options](#mod-visitor)
    -   [Who is Online Options](#mod-who)
    -   [Advanced Options](#mod-advanced)
3.  [Plugin Guide](#plg)
    -   [System Plugin Count](#plg-count)
    -   [System Plugin Clean](#plg-clean)
    -   [System Plugin Online](#plg-online)
4.  [Need More Help?](#more-help)

## <a class="doc-top" name="component-guide"></a>Component

### <a name="control-panel"></a>Control Panel

The **Control Panel** as seen below it is designed to be an easy
starting point, think of it as the components head quarters. While
carrying out tasks you can easily jump from the **Control Panel** to the
different sections and then return before moving onto the next one. *\[Figure-1\]*

![Figure-1](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-cpanel.png "Figure-1"){.coalaweb-docs}

### <a name="visitors"></a>Visitors

The next section is the Visitors section this is where all the visitors
to your site are listed. The visitors are displayed with the following
information.

-   Their IP address
-   Browser Type
-   Browser Version
-   Platform (Operating System)
-   Referer Link
-   The date they visited
-   The time they visited
-   Name assignment (optional)
-   Their Location (Only with the Geo Database Installed)

You also have filter and search options. To filter the visitor
information you have the following options.

-   IP - Click to order descending or again for ascending.
-   Browser - Click to order descending or again for ascending.
-   Browser Version - Click to order descending or again for ascending.
-   Platform - Click to order descending or again for ascending.
-   Date of Visit - Click to order descending or again for ascending.
-   IP Owner- Click to order descending or again for ascending.
-   Location - Click to order descending or again for ascending.

You also have a search box where you can choose to enter
an IP, Date, IP Owner or location to search for specific visitor
information. *\[Figure-2\]*

![Figure-2](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-visitors.png "Figure-2"){.coalaweb-docs}

### <a name="ip-cats"></a>IP Categories

To make it easier to organise your know IPs you can create categories to 
associated them with. For example you could create a category called **Bots**
and then add all the known robots in your **Knownips** list to this category. *\[Figure-3\]*

![Figure-3](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-ip-cats.png "Figure-3"){.coalaweb-docs}

### <a name="knownips"></a>Known IPs

The next section is the **Known IPs** section which contains some powerful tools
for controlling what is counted by **Traffic**.  *\[Figure-4\]*.

![Figure-4](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-knownips-1.png "Figure-4"){.coalaweb-docs}

### <a name="ki-ips"></a>IP Formats

When adding IPs to a Known IP entry you have several options, you can specify an 
IP or IP range in the following formats:

-   Single IP - 192.168.1.1
-   Simple IP Range - 192.168.1.1-192.168.1.255
-   Implied IP Range - 192.168.1.

### <a name="ki-scenarios"></a>Scenarios

**Your Own IP:**

If you just want to keep an eye on your own IP for example you could create a 
new entry give it a **Name** and **Description**
add your **IP** and leave **Count** to yes. Now in the **Visitors** view you
can see your visits easily by look down the **IP Owner** column. *\[Figure-3\]*.

**Block by IP:**

If you want to stop an IP from being counted by **Traffic** create a new entry
give it a **Name** and **Description** add the **IP** and set **Count** to 
no. Now that particular IP will not appear in the visitors list as it is not 
counted by the system any more.

**Block by Name:**

If you want to stop a robot from being counted by **Traffic** based on it's **Name** 
create a new entry give it a **Name** and **Description** add the **Robot Name** and 
set **Count** to no. Now that particular robot will not appear in the visitors 
list as it is not counted by the system any more.

<div class="uk-alert" >Note: The most reliable way to identify visitors is by their IP the name information comes from their <em>user agent string</em> which isn't always supplied.</div>

### <a name="geo"></a>GEO Location

CoalaWeb Traffic gives you the option to identify your visitors **Countries** 
and **Cities** of origin based on their IP addresses. *\[Figure-5\]*.

![Figure-5](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-geo-1.png "Figure-5"){.coalaweb-docs}

#### How Geo Location Works

CoalaWeb Traffic uses the free
[MaxMind's](http://dev.maxmind.com/geoip/geolite) GeoLiteCity database
for determining the country and city information of your visitors. This
file is updated very frequently, about once every month. Why so often?
IP assignments to countries change all the time in fact by the time we
release our extension, the database file is most likely already slightly
out of date.

#### What Will This Affect

This could cause some IP addresses to be identified as coming from the
wrong location. Updating the file regularly will give you much better
country and city accuracy.
[MaxMind](http://dev.maxmind.com/geoip/geolite) claims an accuracy of
99.5% for its free GeoLiteCity database so please bear in mind that this
means that some IP addresses might be reported wrongly.

#### Do I Have To Install It?

**No you do not.** The system will continue to count and store your
website traffic with out the database installed the only difference is
that you won't see *Country* or *City* information associated with their
IP addresses.

<div class="uk-alert">Note: It's a good idea to inform visitors in your privacy policy or TOS that you are collecting their information.</div>

#### <a name="geo-install"></a>Installing the Geo Database

If you don’t have the **GeoLiteCity** database installed you will receive an
notice message. To take advantage of CoalaWeb
Traffics inbuilt ability to tell you a visitors country and sometimes
their city follow the steps below. *\[Figure-5a\]*.

![Figure-5a](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-geo-2.png "Figure-5a"){.coalaweb-docs}

To make it easier to know if you will need to upload the database manually I have added a
**Upload Minimum Requirements** check list that will display in the Geo Location view. *\[Figure-5b\]*.

![Figure-5b](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-geo-3.png "Figure-5b"){.coalaweb-docs}

If your system doesn't meet the minimum requirements but its close I recommend 
trying the easy way first and then moving on the the manual install.
 
#### <a name="geo-easy"></a>Easy Install

First click the **Upload GeoLiteCity Database** blue button this will retrieve the latest version of the
database from the **Maximind** website and upload it to your website's **tmp**
directory. *\[Figure-5c\]*.

![Figure-5c](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-geo-4.png "Figure-5c"){.coalaweb-docs}

If everything went according to plan you will receive a
conformation message that it uploaded correctly. *\[Figure-5d\]*.

![Figure-5d](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-geo-5.png "Figure-5d"){.coalaweb-docs}

The next step is to **Unzip** the file to the CoalaWeb Traffic geoip
directory where it can be accessed and used to determine your visitors
locations. If the database uploaded correctly in the last step you will
now have a **Unzip** icon in the top tool bar click this to start the unzip process. *\[Figure-5e\]*.

![Figure-5e](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-geo-6.png "Figure-5e"){.coalaweb-docs}

Once again if everything goes according to plan you receive a
conformation message that the file was unzipped correctly and also the
message at the top of the page will turn green with today's
date. *\[Figure-5f\]*.

![Figure-5f](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-geo-7.png "Figure-5f"){.coalaweb-docs}

Now CoalaWeb Traffic will automatically add country and city information
to your visitor records as they are collected. To keep the location
information as accurate as possible just carry out this procedure at
regular intervals.

<div class="uk-alert">Note: Please be patient when **Uploading** and <em>Unzipping</em> the database it may take some time due to the size of the file.</div>

#### <a name="geo-manual"></a>Manual Install

If you couldn't install the database the easy way no problem lets just do it the manual
way by following these steps. The sizes I mentions in the following steps may differ but you get the idea.

<div class="uk-alert">Note: To avoid issues please follow these steps exactly as they are written.</div>

Download the latest MaxMind GeoLiteCity database 
[HERE](http://geolite.maxmind.com/download/geoip/database/GeoLiteCity.dat.gz). *\[Figure-5g\]*.

![Figure-5g](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-geo-8.png "Figure-5g"){.coalaweb-docs}

As you can see it should be at least 10.8MB in my case once using Linux when it was
downloaded the system saw it as 11.3MB. *\[Figure-5h\]*.

![Figure-5h](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-geo-9.png "Figure-5h"){.coalaweb-docs}

When extracted my system reports it as 17.6MB *\[Figure-5i\]*.

![Figure-5i](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-geo-10.png "Figure-5i"){.coalaweb-docs}

Now all we are doing is convert the name to lowercase. *\[Figure-5j\]*.

![Figure-5j](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-geo-11.png "Figure-5j"){.coalaweb-docs}

Now don't rezip the file just uploaded it to:

    administrator/components/com_coalawebtraffic/assets/geoip

Now you should have a file 17.7MB in size with 644 permissions in the directory. *\[Figure-5k\]*.

![Figure-5k](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-geo-12.png "Figure-5k"){.coalaweb-docs}

Now if everything went according to plan you should now start to see **Country 
and City** data in the **Visitors** view.


### <a name="export-csv"></a>Export CSV Report

If you want to export the visitors currently stored in your database
start by selecting **Visitors** from the menu bar or from the **Control
Panel**. The main concept you have understand is what you see is what
you get for example if I want all the records for the IP Owner CoalaWeb
I would do the following.

First Type CoalaWeb into the search box and press enter. *\[Figure-6\]*

![Figure-6](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-export-1.png "Figure-6"){.coalaweb-docs}

Now only records with CoalaWeb are listed next choose **All** from the
bottom pagination select box. *\[Figure-6a\]*

![Figure-6a](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-export-2.png "Figure-6a"){.coalaweb-docs}

Now we have all the records with CoalaWeb as the IP owner listed on one
page next click **CSV Report** from the top right menu. *\[Figure-6b\]*

![Figure-6b](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-export-3.png "Figure-6b"){.coalaweb-docs}

You should get a pop up that similar to the image below if not make sure
it's not being blocked by something such as your browser settings. *\[Figure-6c\]*

![Figure-6c](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-export-4.png "Figure-6c"){.coalaweb-docs}

Next save the file to your local computer and then open it with your
application of choice. In this example I will be using LibreOffice but
the procedure will be similar with other applications. First I have to
import it before I can work with the data so after a double click I'm
confronted with the window below. *\[Figure-6d\]*

![Figure-6d](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-export-5.png "Figure-6d"){.coalaweb-docs}

I have chosen to import it with the default settings which results in
the data being laid out in a sheet.  *\[Figure-6e\]*

![Figure-6e](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-export-6.png "Figure-6e"){.coalaweb-docs}

You can now format, filter and save the data as you wish.

<div class="uk-alert">Note: Don't forget what you see is what you get! The exported file will contain what is displayed on the screen.</div>

### <a name="help"></a>Inbuilt Help

In the control panel or the tool menu you have a help icon that when
clicked will open a pop up wrapper of this specific guide. This gives
you an easy way of checking the functionality of a particular item with
out leaving the control panel. *\[Figure-7\]*

![Figure-7](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-help.png "Figure-7"){.coalaweb-docs}

### <a name="options"></a>Extension Options

In the control panel or the tool menu you have a **Options** icon that when
clicked will open a series of extension options.


#### General Options

The first option in this section is the **Locktime** this is the amount of time
that must pass before a particular IP will be counted again. It is
measured in minutes and 1440 (Full day) is the default. *\[Figure-8\]*

The next option is **Week Start** which allows you to choose which day you want
the calculations for the **Weeks** visitors to start from. This only affects the
week count in the front end module and the back end statistics area of the 
control panel. *\[Figure-8\]*

The last option in this section is the **Preset Counter** this number will be 
added to the current **Total** so its good for when you move a site or to bump
up the visitors. This only affects the total count in the front end module and 
the back end statistics area of the control panel. *\[Figure-8\]*

![Figure-8](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-options-1.png "Figure-8"){.coalaweb-docs}

#### Cleanup

In this section you can control the automatic clean up of the database to stop
the tables filling up with data. I recommend having this set to on and the second
option of how many **Records to Keep** will depend on your circumstances. *\[Figure-8a\]*

![Figure-8a](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-options-2.png "Figure-8a"){.coalaweb-docs}

#### Project Honeypot

Project Honeypot is a collective effort to detect spammers, email harversters 
and crackers. Its HTTP:BL service allows participants to query the IP addresses 
of their visitors and figure out if it is a malicious user behind it. If you 
enable this feature, CoalaWeb Traffic will check the IP address of each visitor 
and, if it is a malicious user, it will not count them. *\[Figure-8b\]*

![Figure-8b](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-options-3.png "Figure-8b"){.coalaweb-docs}

<div class="uk-alert">Note: CoalaWeb Traffic does not block visitors from your site only from being counted by the Traffic system.</div>

**Use Project Honeypot**

-   This option is an easy one it turns the feature on and off

**API key**

-   Enter your HTTP:BL key. You can sign up for Project Honeypot and get your 
key at http://www.projecthoneypot.org/httpbl_configure.php.

**Block suspicious**

-   Sometimes Project Honeypot is not sure if an IP belongs to a spammer or 
someone who made a couple of bad decisions while surfing the web. In this case 
the IP is marked as "suspicious". The default behaviour is to not block these IPs. 

**Block Search Engines**

-   If you don't want search engines being counted as visitors to your site you 
can turn this on. This does not guarantee that all search engines won't be 
counted but it's a good start. 

**Minimum Threat (0-255, default 25)**

-   Project Honeypot uses a logarithmic "threat rating" to rank the possibility 
of a specific IP being a spammer. This options defines the minimum threat level 
an IP must have before it's blocked. A value of 25 means that this IP has 
submitted 100 spam messages on Project Honeypot's spam catching honeypots and 
is usually a safe indication that it belongs to a spammer. Do note that the 
rating is logarithmic. A value of 50 means 1,000 spam messages and a value of 
75 means one million spam messages. Do not set it to values over 50, as you 
will most likely never block any spammer at all.

**Maximum Age**

-   Project Honeypot reports when was the last time this IP was caught sending 
spam messages. The older this is (the higher the age is), the less likely is 
that this IP is still used by a spammer. You can chose here what will be the 
maximum reported age that will be blocked. The default value of 30 means that 
IPs which have submitted a spam message in the last 30 days will be blocked.

#### Obsolete

The options in this section are obsolete and have been included to allow users 
an opportunity to transfer them to the new system. *\[Figure-8c\]*

![Figure-8c](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-options-4.png "Figure-8c"){.coalaweb-docs}

#### Permissions

Lastly you have the permissions used to control access to
the CoalaWeb Traffic component. *\[Figure-8d\]*

![Figure-8d](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/cw-traffic-options-5.png "Figure-8d"){.coalaweb-docs}


# <a name="module"></a>CoalaWeb Traffic Module

The CoalaWeb Traffic module has a huge list of options so we have broken
them up into several sections which are explained in detail below.

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