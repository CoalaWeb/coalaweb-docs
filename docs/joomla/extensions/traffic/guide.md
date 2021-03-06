## <a class="doc-top" name="toc">Table of Contents
1.  [Overview](#overview)
2.  [GDPR](#gdpr)
    -   [What is the GDPR?](#gdpr-what)
    -   [CoalaWeb Traffic Data](#gdpr-data)
    -   [Disclaimer](#gdpr-disclaimer)
3.  [Component Guide](#component-guide)
    -   [Control Panel](#control-panel)
    -   [Visitors](#visitors)
    -   [Locations \[Pro\]](#locations)
    -   [IP Categories](#ip-cats)
    -   [Known IPs](#knownips)
        - [1. IP Formats](#ki-ips)
        - [2. Scenarios](#ki-scenarios)
    -   [GEO Manage](#geo)
        - [1. Install](#geo-install)
        - [2. Easy Install](#geo-easy)
        - [3. Manual Install](#geo-manual)
        - [4. Refresh](#geo-refresh)
        - [5. Remove](#geo-remove)
        - [6. MaxMind License Key](#geo-key)
    -   [GEO DB Update \[Pro\]](#geo-update)
    -   [Charts \[Pro\]](#com-charts)
    -   [Help](#help)
    -   [Options](#options)
        - [1. General](#options-general)
        - [2. Storage \[Pro\]](#options-storage)
        - [3. Robots\[Pro\] ](#options-robots)
        - [4. Cleanup](#options-cleanup)
        - [5. Honeypot](#options-honeypot)
        - [6. Charts \[Pro\]](#options-charts)
        - [7. Updates \[Pro\]](https://coalaweb.com/support/documentation/item/updating-guide)
            - [Where is my Download ID?](https://coalaweb.com/support/documentation/item/updating-guide#dl-id)
        - [8. Permissions](#options-permissions)
    -   [Manage](#manage)
        -   [Tools](#man-tools)
            -   [Purge Visitors](#com-purge)
            -   [Purge Locations \[Pro\]](#com-purge-locations)
            -   [Sync Locations \[Pro\]](#com-sync-locations)
            -   [Optimize \[Pro\]](#com-optimize)
            -   [Add Robots \[Pro\]](#com-robots)
        -   [Reports](#man-reports)
            -   [CSV Report](#export-csv)
        -   [Backup \[Pro\]](#man-backup)
        -   [Restore \[Pro\]](#man-restore)
4.  [Traffic \[M\]](#module)
    -   [General](#mod-general)
    -   [Layout](#mod-layout)
    -   [Visitor](#mod-visitor)
    -   [Who is Online](#mod-who)
    -   [Advanced](#mod-advanced)
5.  [Traffic Pro \[M\]](#module-pro)
    -   [General](#mod-pro-general)
    -   [Layout](#mod-pro-layout)
    -   [Traffic](#mod-pro-traffic)
    -   [Visitor](#mod-pro-visitor)
    -   [Who is Online](#mod-pro-who)
    -   [Advanced](#mod-pro-advanced)
6.  [Stats \[A M\]\[Pro\]](#module-traffic-stats)
7.  [Places \[M\]\[Pro\]](#module-places)
8.  [Plugins](#plg)
    -   [System Plugin - Count](#plg-count)
    -   [System Plugin - Clean](#plg-clean)
    -   [System Plugin - Online](#plg-online)
9.  [Need More Help?](#more-help)

## <a name="overview"></a>Overview

**CoalaWeb Traffic** is a Joomla extension designed to keep track of the visitors to your site. You can choose to display the modules and let visitors see and be amazed by your traffic or unpublish the module and view your website statistics in the **Admin** area.

<div class="uk-alert">When installing all the parts of the system will be installed at the same time making installing, upgrading and uninstalling a breeze.</div>

## <a name="gdpr"></a>GDPR

### <a name="gdpr-what"></a>What is the GDPR?

The **General Data Protection Regulation 2016/679** is a regulation in EU law on data protection and privacy for all individuals within the European Union and the European Economic Area. It also addresses the export of personal data outside the EU and EEA. [More at Wikipedia](https://en.wikipedia.org/wiki/General_Data_Protection_Regulation")

### <a name="gdpr-data"></a>CoalaWeb Traffic Data

This extension records visitors' information including their **IP** address.

- **Pro subscribers** have the option to store visitors IPs in a hash (hidden) format which to our knowledge meets the data privacy requirements.

Visitor information is also recorded by the **Who is Online** part of the system which includes an **IP** address and a **Cookie**

- **Pro subscribers** have the option to store visitors IPs in a hash (hidden) format which to our knowledge meets the data privacy requirements.
- There are **two** options in regards to the Cookie. The first is display a message informing users that your website stores and uses Cookies with an accompanying consent button. The second option is set the component option **Set Cookie** to **No** which will remove any current Cookies and stop any new ones from being created.

<div class="uk-alert"> Note: If you choose <strong>Not</strong> to set a <strong>Cookie</strong> the <strong>Who is Online</strong> section will <strong>Not</strong> display in the front end modules.</div>

### <a name="gdpr-disclaimer"></a>Disclaimer

The GDPR is complex topic and the information above is based on our research but is in no way a guarantee that we have covered all aspects of the GDPR and or that CoalaWeb Traffic meets all of it's regulations. If you have more GDPR information, a GDPR related question, have spotted an error or have a GDPR feature request feel free to drop by the [GDPR part of the Forum](https://coalaweb.com/forum/gdpr") and lets us know.

## <a name="component-guide"></a>Component

### <a name="control-panel"></a>Control Panel

The **Control Panel** as seen below it is designed to be an easy starting point, think of it as the components head quarters. While carrying out tasks you can easily jump from the **Control Panel** to the different sections and then return before moving onto the next one. *\[Figure-1\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-cpanel.png">![Figure-1](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-cpanel.png "Figure-1"){.uk-thumbnail .uk-thumbnail-mini}</a>

### <a name="visitors"></a>Visitors

![Figure-2](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-visitors.png "Figure-2"){.uk-thumbnail}


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

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-visitors-1.png">![Figure-2a](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-visitors-1.png "Figure-2a"){.uk-thumbnail .uk-thumbnail-mini}</a>

**Pro** subscribers also get **Filter** options which can be used by clicking the **Search Tools** button at the top and include **Browser**, **Platform** and **Country** select lists. *\[Figure-2b\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-visitors-2.png">![Figure-2b](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-visitors-2.png "Figure-2b"){.uk-thumbnail .uk-thumbnail-mini}</a>

### <a name="locations"></a>Locations \[Pro\]

![Figure-36](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-locations.png "Figure-36"){.uk-thumbnail}

To make it easier to follow I have broken this section up into two parts.

<div class="uk-alert">Note: Unpublished items will continue to be counted but will not display in charts or front end module.</div>

#### Part 1 - List View

The Locations section is where all the locations counts for countries and cities are listed. The locations are displayed with the following information.

-   Status
-   Type
-   Country
-   City
-   Count
-   ID

To sort the location information you can click the column **Heading** or use the **Select list** in the top right. The avaliable sorting options are:

-   Country
-   City
-   Type
-   Count
-   ID

You also have a search box where you can search for specific location information. *\[Figure-36a\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-locations-1.png">![Figure-36a](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-locations-1.png "Figure-36a"){.uk-thumbnail .uk-thumbnail-mini}</a>

**Filter** options are also avaliable which can be used by clicking the **Search Tools** button at the top and include **Status**, **Type** **Country** and **City** select lists. *\[Figure-36b\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-locations-2.png">![Figure-36b](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-locations-2.png "Figure-36b"){.uk-thumbnail .uk-thumbnail-mini}</a>

#### Part 2 - Edit View

Each location listed can be edited and or new locations can be added. In the edit view you can choose if its a **Country** or **City** type, it's **Country** from the list and it's current count. You can also choose if you want the status set to published or not which will stop it from being display in the charts and front end modules but it will continue to be counted. *\[Figure-36c\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-locations-3.png">![Figure-36c](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-locations-3.png "Figure-36c"){.uk-thumbnail .uk-thumbnail-mini}</a>

### <a name="ip-cats"></a>IP Categories

![Figure-3](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-ip-cats.png "Figure-3"){.uk-thumbnail}

To make it easier to organize your **Know IPs** you can create categories to associated them with. For example you could create a category called **Robots** and then add all the known robots in your **Knownips** list to this category. *\[Figure-3a\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-ip-cats-1.png">![Figure-3a](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-ip-cats-1.png "Figure-3a"){.uk-thumbnail .uk-thumbnail-mini}</a>

### <a name="knownips"></a>Known IPs

![Figure-4](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-knownips.png "Figure-4"){.uk-thumbnail}

The next section is the **Known IPs** section which contains some powerful tools for controlling what is counted by **Traffic**.  *\[Figure-4a\]*.

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-knownips-1.png">![Figure-4a](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-knownips-1.png "Figure-4a"){.uk-thumbnail .uk-thumbnail-mini}</a>

### <a name="ki-ips"></a>IP Formats

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-knownips-2.png">![Figure3](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-knownips-2.png "Figure-3"){.uk-thumbnail .uk-thumbnail-mini}</a>

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

### <a name="geo"></a>GEO Manage

CoalaWeb Traffic gives you the option to identify your visitors **Countries** and **Cities** of origin based on their IP addresses. *\[Figure-5\]*.

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-geo-1.png">![Figure-5](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-geo-1.png "Figure-5"){.uk-thumbnail .uk-thumbnail-mini}</a>

#### How Geo Location Works

CoalaWeb Traffic can work in conjunction with **MaxMind's** Geo databases to help determine location information about your visitors. Both the **Core** and **Pro** versions of CoalaWeb Traffic use the **GeoLite2 City** database. The databases are updated very frequently, about once every month. Why so often? IP assignments to countries change all the time in fact by the time we release our extension, the database file is most likely already slightly out of date.

<div class="uk-alert">Note: <a class=\"alert-link\" href="https://blog.maxmind.com/2019/12/18/significant-changes-to-accessing-and-using-geolite2-databases/">MaxMind</a> as of <strong>December 30 2019</strong> now require users to to create an account to access their <strong>GeoLite2</strong> databases. Need help creating a MaxMind account or license key? <a class=\"alert-link\" href="#geo-key">More Info</a></div>

#### What Will This Affect

This could cause some IP addresses to be identified as coming from the wrong location. Updating the file regularly will give you much better country and city accuracy. MaxMind claims an accuracy of 99.5% for its free Geo databases so please bear in mind that this means that some IP addresses might be reported wrongly.

#### Do I Have To Install It?

**No you do not.** The system will continue to count and store your website traffic with out the database installed the only difference is that you won't see *Country* or *City* information associated with their IP addresses.

<div class="uk-alert">Note: It's a good idea to inform visitors in your privacy policy or TOS that you are collecting their information.</div>

### <a name="geo-install"></a>Installing the Geo Database

If you don’t have the **GeoLite2 City** database installed you will receive a notice message. To take advantage of CoalaWeb Traffics inbuilt ability to tell you a visitors country and sometimes their city follow the steps below. *\[Figure-5a\]*.

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-geo-2.png">![Figure5a](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-geo-2.png "Figure-5a"){.uk-thumbnail .uk-thumbnail-mini}</a>

To make it easier to know if you will need to upload the database manually I have added a **Upload Minimum Requirements** check list that will display under the **Requirements** tab. *\[Figure-5b\]*. 

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-geo-3.png">![Figure-5b](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-geo-3.png "Figure-5b"){.uk-thumbnail .uk-thumbnail-mini}</a>

<div class="uk-alert">Don't meet the minimum requirements? The system will attempt to increase the limits temporarily while installing so I recommend giving it a try anyway.</div>
 
#### <a name="geo-easy"></a>Easy Install

<div class="uk-alert">Note: <a class=\"alert-link\" href="https://blog.maxmind.com/2019/12/18/significant-changes-to-accessing-and-using-geolite2-databases/">MaxMind</a> as of <strong>December 30 2019</strong> now require users to to create an account to access their <strong>GeoLite2</strong> databases. Need help creating a MaxMind account or license key? <a class=\"alert-link\" href="#geo-key">More Info</a></div>

1. Login into [MaxMind](https://www.maxmind.com/en/account/login) and create a **License Key**. [More Info](#geo-key)
2. Enter and save your new **License Key** in the component options.

<div class="uk-alert">What happens when I click the <em>Install Geo Database</em> button?</div>

3. The system will retrieve the latest version of the database from the **Maximind** website and upload it to your website's **tmp** directory. 
4. Next the system  will attempt to extract and move it to the CoalaWeb Traffic component location to be used by the system. 
5. Lastly the downloaded file will be deleted from the tmp directory.

Now that we know what happens lets try to install the **Geo Database** by clicking the **Install Geo Database** button. *\[Figure-5c\]*.

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-geo-4.png">![Figure-5c](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-geo-4.png "Figure-5c"){.uk-thumbnail .uk-thumbnail-mini}</a>

If everything goes according to plan you will receive a confirmation message that the file was installed correctly. *\[Figure-5d\]*.

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-geo-5.png">![Figure-5d](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-geo-5.png "Figure-5d"){.uk-thumbnail .uk-thumbnail-mini}</a>

The message under the **Current Version** tab will also turn green and contain today's date. *\[Figure-5e\]*.

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-geo-6.png">![Figure-5e](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-geo-6.png "Figure-5e"){.uk-thumbnail .uk-thumbnail-mini}</a>

Now CoalaWeb Traffic will automatically add country and city information to your visitor records as they are collected. To keep the location information as accurate as possible just carry out this procedure at regular intervals.

<div class="uk-alert">Note: Please be patient when <em>Installing</em> the database it may take some time due to the size of the file.</div>

#### <a name="geo-manual"></a>Manual Install

If you couldn't install the database the easy way no problem lets just do it the manual way by following these steps.

<div class="uk-alert">Note: To avoid issues please follow these steps exactly as they are written.</div>

1. Login into [MaxMind](https://www.maxmind.com/en/account/login). Dont have an account? [More Info](#geo-key)
2. Download the latest MaxMind **GeoLite2 City** database.
3. Now that you have the database downloaded the next step is to extract it. Once it has completed the extraction process you will have a file named **GeoLite2-City.mmdb** *\[Figure-5i-a\]*.

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-geo-10a.png">![Figure-5i-a](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-geo-10a.png "Figure-5i-a"){.uk-thumbnail .uk-thumbnail-mini}</a>

4. Next upload the database file to the following location:

    administrator/components/com_coalawebtraffic/assets/geoip/v2

5. Make sure the database file has **644** permissions. *\[Figure-5k-a\]*.

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-geo-12a.png">![Figure-5k-a](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-geo-12a.png "Figure-5k-a"){.uk-thumbnail .uk-thumbnail-mini}</a>

6. Now if everything went according to plan you should now start to see **Country and City** data in the **Visitors** view.

#### <a name="geo-refresh"></a>Refresh

This option will clear and **regenerate location data** associated with your stored visitors. This can be useful for example after you have updated the GEO database. *\[Figure-5l\]*.

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-geo-14.png">![Figure-5l](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-geo-14.png "Figure-5l"){.uk-thumbnail .uk-thumbnail-mini}</a>

#### <a name="geo-remove"></a>Remove

If you are having problems with the GEO database or no longer want to use the GEO location feature you can use the button in this section to **remove** the GEO database from your system. It's also helpful if you suspect the GEO database if corrupted and you want a clean start before trying to install it again. *\[Figure-5m\]*.

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-geo-15.png">![Figure-5m](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-geo-15.png "Figure-5m"){.uk-thumbnail .uk-thumbnail-mini}</a>

#### <a name="geo-key"></a>MaxMind License Key

So you want to use the easy method of installing and updating your GEO database through the **GEO Manage** section of CoalaWeb Traffic, then as of December 30 2019 you will need a MaxMind account and also create a **License Key**. But don't worry it's easy just follow these steps.

1. Head over to [MaxMind](https://www.maxmind.com/en/geolite2/signup) and create a **GeoLite2** account.
2. Next [Login](https://www.maxmind.com/en/account/login) and click the **My License Key** link in the side menu under **Services**.
3. Now click the **Generate new license key** button and in the next window give it a description and click **Confirm**.
4. You should now see a message confirming the creation of your new license key and more importantly you should see the new key list underneath.
5. Copy the new **Key** over to the CoalaWeb Traffic component options under the **GEO** tab and then save.
6. That's it you have created and saved your new MaxMind license key.

<div class="uk-alert">TIP: To stop any typos I recommend copying and pasting the <strong>License Key</strong> and also to check for no spaces at the end.</div>

### <a name="geo-update"></a>GEO DB Update \[Pro\]

**Pro subscribers** get a button in the control panel called **GEO DB Update** which when pressed will install the latest version of the GEO database. This button makes keeping the GEO DB up to date a quick and easy process which in-turn keeps the location data as accurate as possible. *\[Figure-5n\]*.

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-geo-update.png">![Figure-5n](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-geo-update.png "Figure-5n"){.uk-thumbnail .uk-thumbnail-mini}</a>

### <a name="com-charts"></a>Charts \[Pro\]

Pro subscribers also get access to a series of **Charts** which allow you to quickly see your visitor data grouped in the following ways.

#### Visitors

A quick summary of your visitors displayed in a graph based on quantity and date accompanied by a summary table. *\[Figure-14\]*.

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-chart-1.png">![Figure-14](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-chart-1.png "Figure-14"){.uk-thumbnail .uk-thumbnail-mini}</a>

#### Countries

A color coded map visual representing your visitors and their countries accompanied by a summary table. *\[Figure-14a\]*.

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-chart-2.png">![Figure-14a](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-chart-2.png "Figure-14a"){.uk-thumbnail .uk-thumbnail-mini}</a>

#### Cities

A color coded pie chart representing your visitors and their cities accompanied by a summary table. *\[Figure-14b\]*.

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-chart-3.png">![Figure-14b](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-chart-3.png "Figure-14b"){.uk-thumbnail .uk-thumbnail-mini}</a>

#### Browsers

A color coded pie chart representing your visitors and their browsers accompanied by a summary table. *\[Figure-14c\]*.

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-chart-4.png">![Figure-14c](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-chart-4.png "Figure-14c"){.uk-thumbnail .uk-thumbnail-mini}</a>

#### Platforms

A color coded pie chart representing your visitors and their platforms accompanied by a summary table. *\[Figure-14d\]*.

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-chart-5.png">![Figure-14d](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-chart-5.png "Figure-14d"){.uk-thumbnail .uk-thumbnail-mini}</a>

### <a name="help"></a>Inbuilt Help

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-help-1.png">![Figure-7](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-help-1.png "Figure-7"){.uk-thumbnail .uk-thumbnail-mini}</a>

In the control panel or the tool menu you have a help icon that when clicked will open a pop up wrapper of this specific guide. This gives you an easy way of checking the functionality of a particular item without leaving the control panel. *\[Figure-7a\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-help-2.png">![Figure-7a](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-help-2.png "Figure-7a"){.uk-thumbnail .uk-thumbnail-mini}</a>

### <a name="options"></a>Extension Options

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-options.png">![Figure-8](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-options.png "Figure-8"){.uk-thumbnail .uk-thumbnail-mini}</a>

<div class="uk-alert">In the control panel or the tool menu you have a <em>Options</em> icon that when clicked will open a series of extension options.</div>

#### <a name="options-general"></a>1. General Options

The first option in this section is the **Locktime** this is the amount of time that must pass before a particular IP will be counted again. It is measured in minutes and 1440 (Full day) is the default. *\[Figure-8\]*

The next option is **Week Start** which allows you to choose which day you want the calculations for the **Weeks** visitors to start from. This only affects the week count in the front end module and the back end statistics area of the control panel. *\[Figure-8\]*

The last option in this section is the **Preset Counter** this number will be added to the current **Total** so its good for when you move a site or to bump up the visitors. This only affects the total count in the front end module and the back end statistics area of the control panel. *\[Figure-8a\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-options-1.png">![Figure-8a](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-options-1.png "Figure-8a"){.uk-thumbnail .uk-thumbnail-mini}</a>

#### <a name="options-storage"></a>2. Storage \[Pro\]

The first option in th is section is to turn on or off the storing of IPs in **Raw** format otherwise they will only be stored in an unreadable hash format. If you choose no for this option then in the visitors view **Not Stored Raw!** will be displayed in the IP column and every visitor recorded after that will not have its IP stored in raw format in the database. *\[Figure-8e\]*

The second option is to turn on or off the storing of Geo location information. Even if you are not storing IPs in their raw format you can still have Geo information recorded as long as you have uploaded a Geo database. *\[Figure-8e\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-options-6.png">![Figure-8e](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-options-6.png "Figure-8e"){.uk-thumbnail .uk-thumbnail-mini}</a>

#### <a name="options-robots"></a>3. Robots \[Pro\]

The option in this section will use Joomla's JApplicationWebClient class to block a few well known robots from being counted. This will only detects basic robots if you wish to block additional robots use the KnownIPs list. *\[Figure-8f\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-options-7.png">![Figure-8f](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-options-7.png "Figure-8f"){.uk-thumbnail .uk-thumbnail-mini}</a>

#### <a name="options-cleanup"></a>4. Cleanup

In this section you can control the automatic clean up of the database to stop the tables filling up with data. I recommend having this set to on and the second option of how many **Records to Keep** will depend on your circumstances. *\[Figure-8b\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-options-2.png">![Figure-8b](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-options-2.png "Figure-8b"){.uk-thumbnail .uk-thumbnail-mini}</a>

#### <a name="options-honeypot"></a>5. Project Honeypot

Project Honeypot is a collective effort to detect spammers, email harversters and crackers. Its HTTP:BL service allows participants to query the IP addresses of their visitors and figure out if it is a malicious user behind it. If you enable this feature, CoalaWeb Traffic will check the IP address of each visitor and, if it is a malicious user, it will not count them. *\[Figure-8b\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-options-3.png">![Figure-8b](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-options-3.png "Figure-8b"){.uk-thumbnail .uk-thumbnail-mini}</a>

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

#### <a name="options-charts"></a>6. Charts

The options in this section control the amount of records displayed in the **Charts**. *\[Figure-8c\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-options-8.png">![Figure-8c](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-options-8.png "Figure-8c"){.uk-thumbnail .uk-thumbnail-mini}</a>

#### <a name="options-permissions"></a>8. Permissions

Lastly you have the permissions used to control access tothe CoalaWeb Traffic component. *\[Figure-8d\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-options-5.png">![Figure-8d](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-options-5.png "Figure-8d"){.uk-thumbnail .uk-thumbnail-mini}</a>

### <a name="manage"></a>Manage

The manage area has some handy tools broken up into sections which are explained in detail below.

### <a name="man-tools"></a>Tools

#### <a name="com-purge"></a>Visitor Purge

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-purge1.png">![Figure-32a](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-purge1.png "Figure-32a"){.uk-thumbnail .uk-thumbnail-mini}</a>

The **Purge** button will delete all of the traffic records current stored in the Traffic database tables. To make sure you haven't accidentally press it you will get a popup asking you to confirm your choice. *\[Figure-32b\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-purge2.png">![Figure-32b](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-purge2.png "Figure-32b"){.uk-thumbnail .uk-thumbnail-mini}</a>

After it has completed you get a confirmation message or an error message if it was unable to carry out the task. *\[Figure-32c\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-purge3.png">![Figure-32c](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-purge3.png "Figure-32c"){.uk-thumbnail .uk-thumbnail-mini}</a>

#### <a name="com-purge-locations"></a>Location Purge \[Pro\]

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-purge-locations-1.png">![Figure-32d](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-purge-locations-1.png "Figure-32d"){.uk-thumbnail .uk-thumbnail-mini}</a>

The **Purge** button will delete all of the location records current stored in the Traffic database tables. To make sure you haven't accidentally press it you will get a popup asking you to confirm your choice. *\[Figure-32e\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/w-traffic-purge-locations-2.png">![Figure-32e](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-purge-locations-2.png "Figure-32e"){.uk-thumbnail .uk-thumbnail-mini}</a>

After it has completed you get a confirmation message or an error message if it was unable to carry out the task. *\[Figure-32f\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-purge-locations-3.png.png">![Figure-32f](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-purge-locations-3.png "Figure-32f"){.uk-thumbnail .uk-thumbnail-mini}</a>

#### <a name="com-sync-locations"></a>Sync Locations \[Pro\]

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-sync-locations-1.png">![Figure-37](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-sync-locations-1.png "Figure-37"){.uk-thumbnail .uk-thumbnail-mini}</a>

<div class="uk-alert">This function is only designed to be run once so after it has finished the button will dissappear.</div>

If you have upgrade from a version before the **Location** system was integrated into **CoalaWeb Traffic Pro** or you have counted vistors before turning on locations tracking you can synronize the current vistors to the location counts with this button. To make sure you haven't accidentally press it you will get a popup asking you to confirm your choice. *\[Figure-37a\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-sync-locations-2.png">![Figure-37a](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-sync-locations-2.png "Figure-37a"){.uk-thumbnail .uk-thumbnail-mini}</a>

After it has completed you get a confirmation message or an error message if it was unable to carry out the task. *\[Figure-37b\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-sync-locations-3.png">![Figure-37b](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-sync-locations-3.png "Figure-37b"){.uk-thumbnail .uk-thumbnail-mini}</a>

#### <a name="com-optimize"></a>Optimize and Repair \[Pro\]

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-optimize1.png">![Figure-33a](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-optimize1.png "Figure-33a"){.uk-thumbnail .uk-thumbnail-mini}</a>

Pro subscribers also get an **Optimize** button which will attempt to repair and optimize all the Traffic database tables. To make sure you haven't accidentally press it you will get a popup asking you to confirm your choice. *\[Figure-33b\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-optimize2.png">![Figure-33b](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-optimize2.png "Figure-33b"){.uk-thumbnail .uk-thumbnail-mini}</a>

After it has completed you get a confirmation message or an error message if it was unable to carry out the task. *\[Figure-33c\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-optimize3.png">![Figure-33c](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-optimize3.png "Figure-33c"){.uk-thumbnail .uk-thumbnail-mini}</a>

#### <a name="com-robots"></a>Add Robots \[Pro\]

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-robots-1.png">![Figure-32a](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-robots-1.png "Figure-32a"){.uk-thumbnail .uk-thumbnail-mini}</a>

The **Add Robots** button allows **Pro** subscribers to auto populate the **Known IP** list with a list of known **Robots** instantly stopping them from being counted. To make sure you haven't accidentally press it you will get a popup asking you to confirm your choice. *\[Figure-32b\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-robots-2.png">![Figure-32b](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-robots-2.png "Figure-32b"){.uk-thumbnail .uk-thumbnail-mini}</a>

After it has completed you get a confirmation message or an error message if it was unable to carry out the task. *\[Figure-32c\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-robots-3.png">![Figure-32c](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-robots-3.png "Figure-32c"){.uk-thumbnail .uk-thumbnail-mini}</a>

<div class="uk-alert">The <em>Add Robots</em> system will compare the current list to what you have stored and add any new robots so I recommend running it after each update.</div>

### <a name="man-reports"></a>Reports

#### <a name="export-csv"></a>CSV Report

If you want to export the visitors currently stored in your database start by clicking the **CSV Report** button in the **Control Panel**.

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-export-1.png">![Figure-6](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-export-1.png "Figure-6"){.uk-thumbnail .uk-thumbnail-mini}</a>

You should get a pop up that similar to the image below if not make sure it's not being blocked by something such as your browser settings. *\[Figure-6c\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-export-4.png">![Figure-6c](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-export-4.png "Figure-6c"){.uk-thumbnail .uk-thumbnail-mini}</a>

Next save the file to your local computer and then open it with your application of choice. In this example I will be using **LibreOffice** but the procedure will be similar with other applications. First I have to import it before I can work with the data so after a double click I'm confronted with the window below. *\[Figure-6d\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-export-5.png">![Figure-6d](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-export-5.png "Figure-6d"){.uk-thumbnail .uk-thumbnail-mini}</a>

I have chosen to import it with the default settings which results in the data being laid out in a sheet.  *\[Figure-6e\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-export-6.png">![Figure-6e](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-export-6.png "Figure-6e"){.uk-thumbnail .uk-thumbnail-mini}</a>

You can now format, filter and save the data as you wish.

### <a name="man-backup"></a>Backup \[Pro\]

Pro subscribers have the option to to create a complete backup of all the Traffic database tables including their structure and content which is then exported as a **.sql** formatted file. To create the backup just click the **Backup Database** button and then choose a location to save the generated **.sql** file to. *\[Figure-34\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-backup-1.png">![Figure34](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-backup-1.png "Figure-34"){.uk-thumbnail .uk-thumbnail-mini}</a>

### <a name="man-restore"></a>Restore \[Pro\]

Pro subscribers also have the option to delete the current Traffic data and replace it with a backed up copy. *\[Figure-35\]*

<div class="uk-alert">Note: Only use .sql files created through the Traffic backup system.</div>

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-restore-1.png">![Figure35](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-restore-1.png "Figure-35"){.uk-thumbnail .uk-thumbnail-mini}</a>

To restore just browse to the location of the saved **.sql** file that was created through the Traffic backup system and then click **Restore Database**. You will be prompted by a popup asking you to confirm that you want to replace the current data with a backed-up copy. *\[Figure-35a\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-restore-2.png">![Figure35a](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-restore-2.png "Figure-35a"){.uk-thumbnail .uk-thumbnail-mini}</a>

After you click **Yes, Restore it!** all the data will be replaced by the backed-up copy and on completion you will receive a confirmation message. *\[Figure-35b\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-restore-3.png">![Figure35b](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-restore-3.png "Figure-35b"){.uk-thumbnail .uk-thumbnail-mini}</a>

## <a name="module"></a>CoalaWeb Traffic \[M\]

The CoalaWeb Traffic module has a huge list of options so we have broken them up into several sections which are explained in detail below.

<div class="uk-alert">If you have a multilingual website please leave text fields found through out the module configuration blank and instead use language files to control the text or create a separate module for each language.</div>

### <a name="mod-general"></a>General Display Options

<div class="uk-alert">To make it easy to explain I have broken this section up into two parts.</div>

#### Part 1 Digital Counter

First you can choose if you want to display the digital counter section at all maybe you only want to display individual counters. Next you can choose how many digits you want to be displayed. The last option in this section is to choose a theme for your digital counter. *\[Figure-9\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-mod-general-1.png">![Figure9](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-mod-general-1.png "Figure-9"){.uk-thumbnail .uk-thumbnail-mini}</a>

#### Part 2 Individual Counters

First you can choose if you want to display the individual counters section at all maybe you only want to display a digital counter. The next option is to choose a theme, this will affect which icons are displayed along side the individual counters or you can choose to have no icons. The next option allows you to turn on or off a horizontal line at the bottom of the counter section.

Next you have the ability to turn on or off the display for today, yesterday, this week, this month and total it's up to you which ones you
want to display. Under each of these options is a text box where you can assign a word to be displayed next to the item. *\[Figure-9a\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-mod-general-2.png">![Figure9a](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-mod-general-2.png "Figure-9a"){.uk-thumbnail .uk-thumbnail-mini}</a>

### <a name="mod-layout"></a>Module Layout Options

The first two options control the width of the counter section and the overall module width.

The next option is the module layout you have three options to choose from.

-   **Default** - The vertical layout allows both the counters and visitor info.
-   **Horizontal** - The horizontal layout only allows counters.
-   **Compact** - The compact layout only displays the horizontal text and the total counter.

The next option is the horizontal text this will display to the left of both the horizontal and compact layouts. The last option is the
separator that will display between items in both the horizontal and compact layouts. *\[Figure-10\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-mod-layout-1.png">![Figure10](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-mod-layout-1.png "Figure-10"){.uk-thumbnail .uk-thumbnail-mini}</a>

### <a name="mod-visitor"></a>Visitor Display Options

This section controls what information about the visitor will be displayed within the **Traffic** module. 

<div class="uk-alert">To make it easier to explain I have broken this section into two parts.</div>

#### Part 1

First you can choose if you want to display the visitor information section at all. Next are the **Title** configuration options, you can to choose to display one including the title text, it's format and it's alignment. The next option allows you to turn on or off a horizontal line at the bottom of the visitor section. *\[Figure-11\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-mod-visitor-1.png">![Figure11](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-mod-visitor-1.png "Figure-11"){.uk-thumbnail .uk-thumbnail-mini}</a>

#### Part 2

In this section you have the option to turn on or off the following items as well as choosing their label text.  *\[Figure-11a\]*

-   IP
-   Browser
-   Operating System

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-mod-visitor-2.png">![Figure11a](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-mod-visitor-2.png "Figure-11a"){.uk-thumbnail .uk-thumbnail-mini}</a>

### <a name="mod-who"></a>Who is Online Options

Due to the flaws in the Joomla method of telling who is online I have created my own that uses cookies and a database table to keep track of who is online. The data is then retrieved and displayed in this section of the module.

First you can choose if you want to display the who is online section at all. Next are the **Title** configuration options, you can choose to display them including their title text, their format and alignment. The next option allows you to turn on or off a horizontal line at the bottom of the who is online section. *\[Figure-12\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-mod-who-1.png">![Figure12](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-mod-who-1.png "Figure-12"){.uk-thumbnail .uk-thumbnail-mini}</a>

### <a name="mod-advanced"></a>Advanced Options

The CoalaWeb Traffic module also has a few of what I consider **Advanced Options** such as the option to turn on or off the loading of the **Core CSS** and Pro subscribers can assigning their own **Custom CSS** file by uploading it to:

    media/coalawebtraffic/modules/traffic/css/custom

and then selecting it with the **Custom CSS** option. This next option allows you to display the **Date and Time** at the bottom of the module as well as choosing its **Format**. You can also assign a **Module Class Suffix** or whether to use **Cache** including the **Cache Time** in this section. *\[Figure-13\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-mod-advanced-1.png">![Figure13](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-mod-advanced-1.png "Figure-13"){.uk-thumbnail .uk-thumbnail-mini}</a>

## <a name="module-pro"></a>CoalaWeb Traffic Pro \[M\]

The CoalaWeb Traffic Pro module has a huge list of options so we have broken them up into several sections which are explained in detail below.

<div class="uk-alert">If you have a multilingual website please leave text fields found through out the module configuration blank and instead use language files to control the text or create a separate module for each language.</div>

### <a name="mod-pro-general"></a>General Options

This section controls the outer container style and title plus the digital counter options. 

<div class="uk-alert">To make it easier to explain I have broken this section into two parts.</div>

#### Part 1 Container

The first option in this section is the choice of **Panel** style for the outer container the holds the other sections of the module. The next part is a series of options to control the style and layout of the main container title which includes whether to display it, it's format, alignment and which icon to use next to it. *\[Figure-18a\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-mod-pro-general-1.png">![Figure18a](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-mod-pro-general-1.png "Figure-18a"){.uk-thumbnail .uk-thumbnail-mini}</a>

#### Part 2 Digital Counter

This section cover the display and style of the **Digital** counter. It can be turned on or off as well as the amount of digits to display and its size. There are also four style options to choose from and the size of the margin below can also be selected. *\[Figure-18b\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-mod-pro-general-2.png">![Figure18b](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-mod-pro-general-2.png "Figure-18b"){.uk-thumbnail .uk-thumbnail-mini}</a>

### <a name="mod-pro-layout"></a>Layout Options

This section controls the layout of the different sections of the module and how they are displayed on a variety of screen sizes.

<div class="uk-alert">Width Guide: Desktop = 960px, Tablet = 768px and Mobile = 480px</div>

The three inner sections of the module can be displayed along side each other depending on avaliable screen size or in one column. These setting will be the default but the module being fully responsive will adapt to the current screen size and changes made to it. *\[Figure-18c\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-mod-pro-layout-1.png">![Figure18c](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-mod-pro-layout-1.png "Figure-18c"){.uk-thumbnail .uk-thumbnail-mini}</a>

### <a name="mod-pro-traffic"></a>Traffic Options

This section controls the inner **Traffic** section which contains the individual counters.

<div class="uk-alert">To make it easier to explain I have broken this section into two parts.</div>

#### Part 1 General

The first series of option in this section control the look and feel of the **Traffic** container which includes it's display and panel style. It also has a series of option to change the style and layout of the **Title** displayed at the top of the panel including it's icon. *\[Figure-18d\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-mod-pro-traffic-1.png">![Figure18d](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-mod-pro-traffic-1.png "Figure-18d"){.uk-thumbnail .uk-thumbnail-mini}</a>

#### Part 2 Counters

The next series of options control the alignment and layout of the individual counters. They included the alignment of the counters, their overall size and the width of the three parts that make up each counter. The first part of a counter is the **Icon** then the **Text** and lastly the **Counter**. You can adjust these widths to suit their content and your avaliable space. *\[Figure-18e\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-mod-pro-traffic-2.png">![Figure18e](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-mod-pro-traffic-2.png "Figure-18e"){.uk-thumbnail .uk-thumbnail-mini}</a>

Next are the individual counter options which allow you to turn them on or off, their text, style and lastly which icon to display with the counter. *\[Figure-18f\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-mod-pro-traffic-3.png">![Figure18f](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-mod-pro-traffic-3.png "Figure-18f"){.uk-thumbnail .uk-thumbnail-mini}</a>

### <a name="mod-pro-visitor"></a>Visitor Options

This section controls the inner **Visitors** section which contains the current visitor information.

<div class="uk-alert">To make it easier to explain I have broken this section into two parts.</div>

#### Part 1 General

The first series of option in this section control the look and feel of the **Visitors** container which includes it's display and panel style. It also has a series of option to change the style and layout of the **Title** displayed at the top of the panel including it's icon. *\[Figure-18g\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-mod-pro-traffic-1.png">![Figure18g](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-mod-pro-traffic-1.png "Figure-18g"){.uk-thumbnail .uk-thumbnail-mini}</a>

#### Part 2 Counters

The next series of options control the alignment and layout of the individual counters. They included the alignment of the counters, their overall size and the width of the three parts that make up each counter. The first part of a counter is the **Icon** then the **Text** and lastly the **Counter**. You can adjust these widths to suit their content and your avaliable space. *\[Figure-18h\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-mod-pro-traffic-2.png">![Figure18h](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-mod-pro-traffic-2.png "Figure-18h"){.uk-thumbnail .uk-thumbnail-mini}</a>

Next are the individual counter options which allow you to turn them on or off, their text, style, which icon to display with the counter and for the date counter the date format. *\[Figure-18i\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-mod-pro-visitor-1.png">![Figure18i](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-mod-pro-visitor-1.png "Figure-18i"){.uk-thumbnail .uk-thumbnail-mini}</a>


### <a name="mod-pro-who"></a>Who is Online Options

This section controls the inner **Who Is Online** section which contains the current who is online information.

<div class="uk-alert">To make it easier to explain I have broken this section into four parts.</div>

#### Part 1 General

The first series of option in this section control the look and feel of the **Who Is Online** container which includes it's display and panel style. It also has a series of option to change the style and layout of the **Title** displayed at the top of the panel including it's icon. *\[Figure-18j\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-mod-pro-traffic-1.png">![Figure18j](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-mod-pro-traffic-1.png "Figure-18j"){.uk-thumbnail .uk-thumbnail-mini}</a>

#### Part 2 Counters

The next series of options control the alignment and size of the who is online counter. *\[Figure-18k\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-mod-pro-who-1.png">![Figure18k](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-mod-pro-who-1.png "Figure-18k"){.uk-thumbnail .uk-thumbnail-mini}</a>

#### Part 3 Who Is Online

Next are the **Who Is Online** counter options which allow you to turn it on or off, it's text, style and lastly which icon to display with the counter.  *\[Figure-18l\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-mod-pro-who-2.png">![Figure18l](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-mod-pro-who-2.png "Figure-18l"){.uk-thumbnail .uk-thumbnail-mini}</a>

#### Part 4 Flags

Next are the **Flag** options which allow you to turn them on or off, the maximum amount to display, their alignment and the section's related title option. *\[Figure-18m\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-mod-pro-who-3.png">![Figure18m](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-mod-pro-who-3.png "Figure-18m"){.uk-thumbnail .uk-thumbnail-mini}</a>

### <a name="mod-pro-advanced"></a>Advanced Options

The CoalaWeb Traffic Pro module also has a few of what I consider **Advanced Options** such as which **UIkit prefix** to use, by default it is set to **CW** but if you are using a **YooTheme** template you may want to change it to **UK**. You can also assign a **Module Class Suffix** or whether to use **Cache** including the **Cache Time** in this section. *\[Figure-18n\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-mod-pro-advanced-1.png">![Figure18n](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/cw-traffic-mod-pro-advanced-1.png "Figure-18n"){.uk-thumbnail .uk-thumbnail-mini}</a>

## <a name="plg"></a>Plugins

<div class="uk-alert">There are several plugins crucial to the proper functioning of the CoalaWeb Traffic system. They are explain in detail below.</div>

### <a name="plg-count"></a>System Plugin - Count

This plugin is crucial to functionality of the system it quietly counts the visits to your site and then records them in the database. It allows you to count the traffic to your site even with the module unpublished and also ensures all traffic is record regardless of the part of the site that they visit.

This plugin also takes care of blocking visitors from being counted based on your setting in the CoalaWeb Traffic component.  *\[Figure-15\]*

<div class="uk-alert">Note: To ensure proper functionality of CoalaWeb Traffic please make sure this plugin is installed and publish.</div>

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/system-parts/traffic-plg-count.png">![Figure15](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/system-parts/traffic-plg-count.png "Figure-15"){.uk-thumbnail .uk-thumbnail-mini}</a>

### <a name="plg-clean"></a>System Plugin - Clean

This plugin carries out the automatic database clean up but only if you have it turned on in the **Component Options**. It will run in the
background keeping the current data but delete out the old entries and add them to a running total. It is recommended to turn this feature
on.   *\[Figure-16\]*

<div class="uk-alert">Have you chosen automatic database clean up? Then this plugin needs to be installed and published.</div>

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/system-parts/traffic-plg-clean.png">![Figure16](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/system-parts/traffic-plg-clean.png "Figure-16"){.uk-thumbnail .uk-thumbnail-mini}</a>

### <a name="plg-online"></a>System Plugin - Online

This plugin will check who is online, record it to a cookie and to the database and lastly supply the information to the **Traffic** modules so they can display the currently online visitors. *\[Figure-17\]*

<div class="uk-alert">Have you chosen to display <em>Who is Online?</em> Then this plugin needs to be installed and published.</div>

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/system-parts/traffic-plg-online.png">![Figure17](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/traffic/system-parts/traffic-plg-online.png "Figure-17"){.uk-thumbnail .uk-thumbnail-mini}</a>

## <a name="more-help"></a>Need More Help

<div class="uk-alert">Do you have a question that wasn't covered by this GUIDE? Try the <a href="https://coalaweb.com/support/documentation/category/traffic" target="_self">FAQ</a></div>

<div class="uk-alert">Do you have a question that wasn't covered by this GUIDE or the FAQ? Then it's time to drop by the <a href="https://coalaweb.com/forum/index" target="_self">Forum</a></div>