## Table of Contents
1.  [Overview](#overview)
2.  [Updates](#updates)
    - [Where is my Download ID?](#options-downloadid)
3.  [Instructions](#instructions)
4.  [Options](#options)
5.  [Need More Help?](#more-help)

## <a class="doc-top" name="overview"></a>Overview

**CoalaWeb Date** gives Joomla administrators the power to display the current **Date** and **Year** in their Joomla content. **Pro** subscribers can **Format** the date for each use and or add **Copyright** information to any Joomla content item.

<div class="uk-alert">When installing all the parts of the system will be installed at the same time making installing, upgrading and uninstalling a breeze.</div>

## <a name="updates"></a>Updates

The **CoalaWeb Date** extension integrates with the inbuilt **Joomla Update** system so both **Core** and **Pro** users can keep their extension up to date. For **Core** users when you see updates listed in the Joomla update manager feel free to select it and update. 

For **Pro** subscribers you will need to make sure you still have a valid subscription and that you have entered your **Download ID** into the **System - CW Gears** plugin. *\[Figure-1\]*

<div class="uk-alert">Not sure where to find your Download ID? Click <a href="#options-downloadid">HERE</a> for more info.</div>

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/gears/cw-gears-f9.png">![Figure-1](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/gears/cw-gears-f9.png "Figure-1"){.uk-thumbnail .uk-thumbnail-mini}</a>

Inside the **CW Gears** plugin options your will find a tab titled **Updates** and under it a **Download ID** input field. I recommend you copy and paste your **Download ID** into this field to reduce the risk of a typo and also to check for no spaces at the end.  *\[Figure-1a\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/gears/cw-gears-f10.png">![Figure-1a](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/gears/cw-gears-f10.png "Figure-1a"){.uk-thumbnail .uk-thumbnail-mini}</a>

<div class="uk-alert">The CW Gears plugin will take care of the Download ID for any CoalaWeb extensions that doesn't come with a component.</div>

#### <a name="options-downloadid"></a> Where can I find my Download ID?

To see your **Download ID** you will need to log into [coalaweb.com](https://coalaweb.com) and then go to:

    Members -> My Subscriptions

You will then see the ID displayed in the module titled **Download ID**. *\[Figure-1b\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/general/updates/cw-updates-download-id.png">![Figure-1b](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/general/updates/cw-updates-download-id.png "Figure-1b"){.uk-thumbnail .uk-thumbnail-mini}</a>

<div class="uk-alert">TIP: To stop any typos I recommend copying and pasting the download ID and also to check for no spaces at the end.</div>

## <a name="instructions"></a>Instructions

####Core and Pro

To display the current date use the plugin code **{cwdate date}** or for the current year use **{cwdate year}** in your joomla content items such as articles and or custom modules.

####Pro Only

To display the current date use the plugin code **{cwdate date}** or in a specific format use **{cwdate date LC4}**. 

####Date Formats: 

- <em>LC1</em> = Saturday, 27 October 2017
- <em>LC2</em> = Saturday, 27 October 2017 12:40
- <em>LC3</em> = 27 October 2017
- <em>LC4</em> = 2017-10-27
- <em>JS1</em> = 17-10-27
- <em>LC4US</em> = 2017-27-10
- <em>JS1US</em> = 17-27-10
- <em>LC4R</em> = 27-10-2017
- <em>JS1R</em> = 27-10-17
- <em>LC4RUS</em> = 10-27-2017
- <em>JS1RUS</em> = 10-27-17

To display copyright information use the plugin code **{cwdate copy}**

<div class="uk-alert">TIP: When using the plugin code in a custom module make sure that the <em>Prepare Content</em> option is set to <em>Yes</em>.</div>

### <a name="options"></a>Options

To make it easier to follow I have broken up this section into two parts.
 
#### Date

In this section you can choose what format you want the date to display in. **Core** users have **4** options while **Pro** subscribers have **11** options to choose from.

The options with a **(J)** come from the core **Joomla** language files. The options with a **(CW)** are extended options provided by **CoalaWeb** and are contained in this extension's language file. *\[Figure 2\]*
                                                                                            
<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/date/cw-date-f1.png ">![Figure-2](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/date/cw-date-f1.png "Figure-2"){.uk-thumbnail .uk-thumbnail-mini}</a>

#### Copyright 

**Pro** subscribers also get the option to display **Copyright** information quickly and easily. The first option allows you to add a predefined **From Year** to be display before the current one but if you don't want one just leave this field blank.

The copyright text comes from a language string in the CoalaWeb Date extension's language files. The current website name as defined in your Joomla settings and the website root will be substitued into the copyright text unless you want to custimize them. To customize either of these items select **Custom** and a new custom field will appear allowing you to enter a website name and or a complete URL for **Name Link**. If you don't want the name to be a link you can also set the **Name Link** option to none. *\[Figure 2a\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/date/cw-date-f2.png ">![Figure-2a](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/date/cw-date-f2.png "Figure-2a"){.uk-thumbnail .uk-thumbnail-mini}</a>


## <a name="more-help"></a>Need More Help

<div class="uk-alert">Do you have a question that wasn't covered by this GUIDE? Then it's time to drop by the <a href="https://coalaweb.com/forum/index" target="_self">Forum</a></div>