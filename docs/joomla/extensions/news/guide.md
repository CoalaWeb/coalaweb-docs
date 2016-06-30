## Table of Contents
1.  [Overview](#overview)
2.  [Updates](#updates)
    - [Where is my Download ID?](#options-downloadid)
3.  [Module News](#mod-news)
    -   [General Options](#mod-general)
    -   [Layout Options](#mod-layout)
    -   [Image Options](#mod-images)
    -   [Details Options](#mod-details)
    -   [Advanced Options](#mod-advanced)
4.  [Need More Help?](#more-help)

## <a class="doc-top" name="overview"></a>Overview

**CoalaWeb News** gives you the power to display your Joomla articles in variety of different ways with completely responsive layouts covering desktops, tablets, and mobile devices plus a tonne of other options. There are two versions available a Core (Free) and Pro (Paid Subscription) version that comes with extend functionality.

<div class="uk-alert">When installing all the parts of the system will be installed at the same time making installing, upgrading and uninstalling a breeze.</div>

## <a name="updates"></a>Updates

The CoalaWeb News extension integrates with the inbuilt **Joomla Update** system so both **Core** and **Pro** users can keep their extension up to date. For **Core** users when you see updates listed in the Joomla update manager feel free to select it and update. 

For **Pro** subscribers you will need to make sure you still have a valid subscription and that you have entered your **Download ID** into the **System - CW Gears** plugin. *\[Figure-11\]*

<div class="uk-alert">Not sure where to find your Download ID? Click <a href="#options-downloadid">HERE</a> for more info.</div>

![Figure-11](http://cdn.coalaweb.com/images/docs/joomla-extensions/gears/cw-gears-f9.png "Figure-11"){.coalaweb-docs}

Inside the **CW Gears** plugin options your will find a tab titled **Updates** and under it a **Download ID** input field. I recommend you copy and paste your **Download ID** into this field to reduce the risk of a typo and also to check for no spaces at the end.  *\[Figure-11a\]*

![Figure-11a](http://cdn.coalaweb.com/images/docs/joomla-extensions/gears/cw-gears-f10.png "Figure-11a"){.coalaweb-docs}

<div class="uk-alert">The CW Gears plugin will take care of the Download ID for any CoalaWeb extensions that doesn't come with a component.</div>

#### <a name="options-downloadid"></a> Where can I find my Download ID?

To see your **Download ID** you will need to log into [coalaweb.com](http://coalaweb.com) and then go to:

    Members -> My Subscriptions

You will then see the ID displayed in the module titled **Download ID**. *\[Figure-11b\]*

![Figure-11b](http://cdn.coalaweb.com/images/docs/joomla-extensions/general/updates/cw-updates-download-id.png "Figure-11b"){.coalaweb-docs}

<div class="uk-alert">TIP: To stop any typos I recommend copying and pasting the download ID and also to check for no spaces at the end.</div>

## <a name="mod-news"></a>News Module

The **CoalaWeb News** module has a huge list of options so we have broken them up into several sections which are explained in detail below.

### <a name="mod-general"></a>General Options

To make it easy to explain I have broken this section up into four parts.

**Part 1 Categories**

The first option you have in this section allows you to choose which categories you want to use as the source for your displayed articles. *\[Figure-1a\]*

![Figure-1a](http://cdn.coalaweb.com/images/docs/joomla-extensions/news/cw-news-mod-general-1a.png "Figure-1a"){.coalaweb-docs}

The second option allows you to display a linked list of categories that coincides with the current articles being displayed. *\[Figure-1b\]*

![Figure-1b](http://cdn.coalaweb.com/images/docs/joomla-extensions/news/cw-news-mod-general-1b.png "Figure-1b"){.coalaweb-docs}

**Part 2 Articles**

The first options allows you to turn on or off the display of an article title. Next you have the option of making the title a link to the associated article or not. With the next option you can select a style for the article title. 

In the next input field you can enter a number to control the maximum amount of articles you wish to be displayed. The next option allows you to control the maximum amount of characters that will be displayed for each article. The next two options affect the ordering of the articles. The last option is for excluding articles from being displayed, just enter the article ID's separated by a comma to have them excluded. *\[Figure-2\]*

![Figure-2](http://cdn.coalaweb.com/images/docs/joomla-extensions/news/cw-news-mod-general-2.png "Figure-2"){.coalaweb-docs}

**Part 3 Read More**

<div class="uk-alert">Note: The Read More code used in your articles will need to be in the following format.</div>

    <hr id="system-readmore" />

In this section we have some options to control if and how a read more link or button will be displayed. The first option is to turn on or off the display of a read more link. The second option control what text will be used for the link or button. 

The next couple of options depends on what version you are using, for the **Core** users you only have a **link** option available. For the **Pro** users you have the **following options**:

-   Button Primary
-   Button Success
-   Button Danger
-   Just Link
-   Custom

The button options above are controlled by UIkit but if you are a **Pro** user and would like to use your own CSS class then chose **Custom** for the **Type** and then enter the CSS class in the next field labeled **Custom Button**. *\[Figure-3\]*

Below is an example CSS class.

>   btn btn-primary

![Figure-3](http://cdn.coalaweb.com/images/docs/joomla-extensions/news/cw-news-mod-general-3.png "Figure-3"){.coalaweb-docs}

**Part 4 Links**

CoalaWeb News also gives you the option to display links to more articles. The first option in this section turns on or off the links section. The second option allows you to enter a number for the amount of links you want displayed.

Next you can chose to display a heading for this section and also select a style for it from the drop down list. The last option allows you to turn on or off the display of a creation date next to each link. *\[Figure-4\]*

![Figure-4](http://cdn.coalaweb.com/images/docs/joomla-extensions/news/cw-news-mod-general-4.png "Figure-4"){.coalaweb-docs}

### <a name="mod-layout"></a>Module Layout Options

To make it easy to explain I have broken this section up into 4 parts.

**Part 1 General**

The first option in this section allows you to choose a layout for the module. If you are a **Core** user you get to use the default layout which is very flexible and for **Pro** subscribers you will get several options to choose from including the default. The next option controls the style of the panel used to contain your individual articles. If you are a **Core** user you get to use the default panel and for **Pro** subscribers you will get several options to choose from including the default.

The next two options affect the margins used by the module. The first option affects the spacing around and between panels and the second affects the spacing within each individual panel. *\[Figure-5\]*

![Figure-5](http://cdn.coalaweb.com/images/docs/joomla-extensions/news/cw-news-mod-layout-1.png "Figure-5"){.coalaweb-docs}

**Part 2 Dynamic Filter**

Pro subscribers get the option to display a menu at the top of the module made up of the categories of the currently display articles. If one of these menu items is selected than the articles will dynamically rearranged to only display the articles that belong to that particular category. *\[Figure-12\] and \[Figure-12a\]*

![Figure-12](http://cdn.coalaweb.com/images/docs/joomla-extensions/news/cw-news-mod-layout-4.png "Figure-12"){.coalaweb-docs}

![Figure-12a](http://cdn.coalaweb.com/images/docs/joomla-extensions/news/cw-news-mod-layout-5.png "Figure-12a"){.coalaweb-docs}

**Part 3 Alignment**

Depending on what settings you choose and how you want your individual panels to look you might want to tweak the alignment of different elements. This next section will help you get the panels looking just how you want by allowing you to align the **Title**, **Details**, **Article Text** and the **Read More** link. *\[Figure-6\]*

![Figure-6](http://cdn.coalaweb.com/images/docs/joomla-extensions/news/cw-news-mod-layout-2.png "Figure-6"){.coalaweb-docs}

**Part 4 Columns**

<div class="uk-alert">Width Guide: Desktop = 960px, Tablet = 768px and Mobile = 480px</div>

The first option in this section is to turn on or off the matching of **Column Heights**. This will make all the displayed columns the height of the largest one making them balanced and symmetrical.

You can also choose how many columns you want to use with the added power to choose based on the size of the screen being used. You can for example have three columns on a nice big desktop screen and then one column on a small mobile device. 

These settings are fully responsive which you can test by minimizing your browser screen on your desktop to simulate different screen sizes and see the changes live. *\[Figure-7\]*

![Figure-7](http://cdn.coalaweb.com/images/docs/joomla-extensions/news/cw-news-mod-layout-3.png "Figure-7"){.coalaweb-docs}

### <a name="mod-images"></a>Image Options

This section is dedicated to the display of images with your article content and contains some powerful features to get your content looking just how you want it. 

To make it easy to explain I have broken this section up into 3 parts.

**Part 1 General**

<div class="uk-alert">All the options below with affect the default layout but may only partially affect certain other layouts. This is to preserve their intended look and feel.</div>

The first option option is an easy one it allows you to turn on or off the display of images. The next option allows you to choose which type of article image to use either the **Intro** or **Full** article image. The next option is to turn on the display of any **Captions** you have added to your article images. *\[Figure-8\]*

![Figure-8](http://cdn.coalaweb.com/images/docs/joomla-extensions/news/cw-news-mod-images-1a.png "Figure-8"){.coalaweb-docs}

**Part 2 Widths**

<div class="uk-alert">Width Guide: Desktop = 960px, Tablet = 768px and Mobile = 480px</div>

In this section you can choose how much space you want your images to use within the panel with the added power to choose based on the size of the screen being used. These settings are fully responsive which you can test by minimizing your browser screen on your desktop to simulate different screen sizes and see the changes live.  *\[Figure-8a\]*

![Figure-8a](http://cdn.coalaweb.com/images/docs/joomla-extensions/news/cw-news-mod-images-2.png "Figure-8a"){.coalaweb-docs}

### Example Scenario

**Desktop:** When viewing the module on a desktop I want one item per column with the image to the side of the panel. *\[Figure-8b\]*

**Settings**
-   Image: Yes
-   Caption: Yes
-   Width on Desktop: 30%
-   Columns on Desktop: 1
-   Layout: Compact Square
-   Panel Style: Secondary

![Figure-8b](http://cdn.coalaweb.com/images/docs/joomla-extensions/news/cw-news-mod-images-3.png "Figure-8b"){.coalaweb-docs}

**Tablet:** When viewing the module on a tablet I want two items per column with the image at the top of the panel. *\[Figure-8c\]*

**Settings**
-   Image: Yes
-   Caption: Yes
-   Width on Tablet: 100%
-   Columns on Tablet: 2
-   Layout: Compact Square
-   Panel Style: Secondary

![Figure-8c](http://cdn.coalaweb.com/images/docs/joomla-extensions/news/cw-news-mod-images-4.png "Figure-8c"){.coalaweb-docs}

**Mobile:** When viewing the module on a tablet I want one item per column with the image at the top of the panel. *\[Figure-8d\]*

**Settings**
-   Image: Yes
-   Caption: Yes
-   Width on Mobile: 100%
-   Columns on Mobile: 1
-   Layout: Compact Square
-   Panel Style: Secondary

![Figure-8d](http://cdn.coalaweb.com/images/docs/joomla-extensions/news/cw-news-mod-images-5.png "Figure-8d"){.coalaweb-docs}

**Part 2 Alignment**

The last option in this section controls the alignment of the images within their allocated space. *\[Figure-8e\]* 

![Figure-8e](http://cdn.coalaweb.com/images/docs/joomla-extensions/news/cw-news-mod-images-6.png "Figure-8e"){.coalaweb-docs}

To make this more clear I will give you an example of left, center and right.

**Left** *\[Figure-8f\]*

![Figure-8f](http://cdn.coalaweb.com/images/docs/joomla-extensions/news/cw-news-mod-images-7.png "Figure-8f"){.coalaweb-docs}

**Center** *\[Figure-8g\]*

![Figure-8g](http://cdn.coalaweb.com/images/docs/joomla-extensions/news/cw-news-mod-images-8.png "Figure-8g"){.coalaweb-docs}

**Right** *\[Figure-8h\]*

![Figure-8h](http://cdn.coalaweb.com/images/docs/joomla-extensions/news/cw-news-mod-images-9.png "Figure-8h"){.coalaweb-docs}

This setting becomes more useful when using a multi column layout and you have small images being display at the top of their panels. *\[Figure-8i\]*

![Figure-8i](http://cdn.coalaweb.com/images/docs/joomla-extensions/news/cw-news-mod-images-10.png "Figure-8i"){.coalaweb-docs}
 
### <a name="mod-details"></a>Details Options

In this section you have the ability to turn on or off a variety of article details for example the **Author**, **Category**, **Creation Date** and or it's amount of **Hits**.  You can also display an accompanying **Title** or turn on or off the section completely. *\[Figure-9\]*

<div class="uk-alert">Note: The location of the article details will be affected by the <em>Layout</em> you have chosen.</div>

![Figure-9](http://cdn.coalaweb.com/images/docs/joomla-extensions/news/cw-news-mod-details-1.png "Figure-9"){.coalaweb-docs}

### <a name="mod-advanced"></a>Advanced Options

The CoalaWeb News module also has a few of what I consider **Advanced Options** such as the UIkit prefix option for when you are using a YooTheme template you can set it to **UK** otherwise I recommend leaving it with the default **CW**. In this section you can also choose to not have HTML striped out of the articles text as well as the option to assign a **Module Class Suffix** and choose whether to use **Cache** including the **Cache Time**. 

<div class="uk-alert">If you have chosen to leave HTML in your articles you will need to have PHP Tidy installed to ensure it's correct functionality.</div>

![Figure-10](http://cdn.coalaweb.com/images/docs/joomla-extensions/news/cw-news-mod-advanced-1.png "Figure-10"){.coalaweb-docs}

## <a name="more-help"></a>Need More Help

<div class="uk-alert">Do you have a question that wasn't covered by this GUIDE? Then it's time to drop by the <a href="http://coalaweb.com/forum/index" target="_self">Forum</a></div>