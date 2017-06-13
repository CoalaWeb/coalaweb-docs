## Table of Contents
1.  [Overview](#overview)
2.  [Updates](#updates)
    - [Where is my Download ID?](#options-downloadid)
3.  [Instructions](#instructions)
4.  [Options](#options)
5.  [Need More Help?](#more-help)

## <a class="doc-top" name="overview"></a>Overview

**CoalaWeb Versions** gives Joomla administrators the power to display their minimum supported versions plus retrieve and display current versions in any Joomla content item. It comes packed with options making it very flexible.

<div class="uk-alert">When installing all the parts of the system will be installed at the same time making installing, upgrading and uninstalling a breeze.</div>

## <a name="updates"></a>Updates

The **CoalaWeb Versions** extension integrates with the inbuilt **Joomla Update** system so both **Core** and **Pro** users can keep their extension up to date. For **Core** users when you see updates listed in the Joomla update manager feel free to select it and update. 

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

#### Core and Pro

To retrieve and display the current Joomla version use the plugin code **{cwversions joomla-current}** or for your currently supported Joomla version as defined in the plugin options use **{cwversions joomla}** in any of your joomla content items such as articles and or custom modules.

#### Pro Only

Pro subscribers also get the following plugin code options:

##### Basic
- Display minimum PHP version **{cwversions php}**
- Display minimum MySQL **{cwversions mysql}**
- Display minimum Browser **{cwversions browser}**

##### Custom
- Display custom options with custom plus number **{cwversions custom1}**

##### Advanced
Pro subscribers also get what I consider advanced options to display the current version of a locally installed extension or via it's update XML file.

- Display currently installed version use it's **element** name **{cwversions element coalawebversions}**
- Display version based on update XML file use **xml** **{cwversions xml http://cdn.coalaweb.com/updates/cw-versions-pro.xml}**

<div class="uk-alert">TIP: If you are using the plugin code in a custom module make sure that the <em>Prepare Content</em> option found under the module's <em>Options</em> tab is set to <em>Yes</em>.</div>

### <a name="options"></a>Options

To make it easier to follow I have broken up this section into two parts.
 
#### Main

In the **Main Options** tab there is a **Joomla** input field for both **Core** and **Pro** users which will display when using the plugin code **joomla**. For **Pro** subscribers there is also **PHP**, **MySQL** and **Browser** input fields. Keep in mind whatever you put in these fields will be displayed when using their corresponding plugin code. *\[Figure 2\]*

#### Examples
- Joomla 3.6+
- PHP 5.4+
- MySQL 5.1+
- Modern Browser (IE >= 9)

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/versions/cw-versions-f1.png ">![Figure-2](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/versions/cw-versions-f1.png "Figure-2"){.uk-thumbnail .uk-thumbnail-mini}</a>

#### Custom \[Pro\]

In the **Custom Options** tab there are three custom input fields which will display when using the plugin code **custom** plus it's corresonding number for example **{cwversions custom1}**. Keep in mind whatever you put in these fields will be displayed. *\[Figure 2a\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/versions/cw-versions-f2.png ">![Figure-2a](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/versions/cw-versions-f2.png "Figure-2a"){.uk-thumbnail .uk-thumbnail-mini}</a>

## <a name="more-help"></a>Need More Help

<div class="uk-alert">Do you have a question that wasn't covered by this GUIDE? Then it's time to drop by the <a href="https://coalaweb.com/forum/index" target="_self">Forum</a></div>