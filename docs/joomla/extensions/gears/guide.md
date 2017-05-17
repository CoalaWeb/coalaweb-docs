## Table of Contents
1.  [Overview](#overview)
2.  [Options](#options)
    -   [General](#opt-general)
    -   [jQuery](#opt-jquery)
    -   [Async](#opt-async)
    -   [Uikit](#opt-uikit)
    -   [Custom CSS](#opt-css)
    -   [Custom JS](#opt-js)
    -   [Cache](#opt-cache)
    -   [Assets](#opt-assets)
    -   [Updates \[Pro\]](#opt-updates)
        - [Where is my Download ID?](#opt-downloadid)
3.  [Need More Help?](#more-help)

## <a class="doc-top" name="overview"></a>Overview

**CoalaWeb Gears** is a Swiss army knife full of great little tools that you can use with or without a CoalaWeb extension.

<div class="uk-alert">When installing all the parts of the system will be installed at the same time making installing, upgrading and uninstalling a breeze.</div>

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/general/generic/coalaweb-tooltip.png">![Figure-Tooltip](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/general/generic/coalaweb-tooltip.png "Figure-Tooltip"){.uk-thumbnail .uk-thumbnail-mini}</a>

## <a name="options"></a>Options

The CoalaWeb Gears plugin has a long list of options so we have broken them up into 8 sections which are explained in detail below.

### <a name="opt-general"></a>General

In the **General** section you have several options the first helps when using **Zoo** by YooTheme by expanding the editor window, making it easier to work on your content. The second option will display a demo of what your system messages will look like, which is great for customizing their style and layout. 

The next option **Gzip help** is designed to help with a know issue where Facebook is unable to access some Joomla sites while using Gzip compression. Not to go into to much detail but it has to do with Facebook only looking at a certain amount of a page and it is misinterpreting some Gzipped sites as being too large. If you turn this option on it will try to detect Facebook and Linking bots and disable Gzip for the duration of their visit. 

Next is the **reCAPTCHA Compact** option which gives you the ability to display the captcha produced by the inbuilt Joomla reCAPTCHA plugin in either a **Standard** or **Compact** layout. The last option is to turn on or off the logging of SQL errors which is very useful for debugging. *\[Figure 1\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/gears/cw-gears-f1.png">![Figure-1](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/gears/cw-gears-f1.png "Figure-1"){.uk-thumbnail .uk-thumbnail-mini}</a>

### <a name="opt-jquery"></a>jQuery

This section is designed to help you safely included jQuery on your site with a few cool features. You can choose to load a local copy or from a remote location such as Google's CDN. You can choose which version to included and also if you want **No Conflict** and or **Migrate** turned on. *\[Figure 2\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/gears/cw-gears-f2.png">![Figure-2](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/gears/cw-gears-f2.png "Figure-2"){.uk-thumbnail .uk-thumbnail-mini}</a>

### <a name="opt-async"></a>Async

**Why use async?**
> What you are trying to prevent with the async attribute is parser blocking. If you use the async attribute, you are saying: I don't want the browser to stop what it's doing while it's downloading this script. I know that this script doesn't really depend on anything being ready in the DOM when it runs and it also doesn't need to be run in any particular order.

**Why user defer?**
> Basically, defer tells the browser to wait "until it's ready" before executing the JavaScript in that script block. Usually this is after the DOM has finished loading.

In this section you can decided if you want to add **Asnyc** and or **Defer** to your scripts including an input box to choose which scripts should be included. *\[Figure 3\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/gears/cw-gears-f3.png">![Figure-3](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/gears/cw-gears-f3.png "Figure-3"){.uk-thumbnail .uk-thumbnail-mini}</a>

### <a name="opt-uikit"></a>Uikit

In this section you have the option to turn on a CoalaWeb specific version of Uikit by YooTheme including an option to choose which of the default themes to use. *\[Figure 4\]*

<div class="uk-alert">This option is only going to apply to a select group of CoalaWeb extensions. Unless otherwise asked to I recommend leaving this option set to <em>Yes</em> to ensure certain CoalaWeb extensions function correctly.</div>

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/gears/cw-gears-f4.png">![Figure-4](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/gears/cw-gears-f4.png "Figure-4"){.uk-thumbnail .uk-thumbnail-mini}</a>

### <a name="opt-css"></a>Custom CSS

In this section you have the option to add custom CSS to your website which is great for testing and small tweaks. *\[Figure 5\]*

You can choose to include code added to the **Custom Code** input field and then you have a few options to make small changes to it before it's included in your website. You can **Minimize** it to make it load as fast as possible also with the option to **Remove Comments** on the fly.

The **Full Paths** option will convert the short version of a used URL to it's full length version. Let me give you an example:
 
    /templates/protostar/images/background.jpg

will become 

    http://www.example.com/templates/protostar/images/background.jpg


<div class="uk-alert"> Note: If turned on make sure to use paths starting from your Joomla root for example <em>/images/backgrounds/my-background.jpg</em></div>

You can also include a **Custom File** if needed, just enter the location of the file you wish to include in the following format.

    /media/mycss/custom.css

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/gears/cw-gears-f5.png">![Figure-5](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/gears/cw-gears-f5.png "Figure-5"){.uk-thumbnail .uk-thumbnail-mini}</a>

### <a name="opt-js"></a>Custom JS

In this section you have the option to add custom JS to your website which is great for testing and small tweaks. *\[Figure 6\]*

You can choose to include code added to the **Custom Code** input field and then you have a few options to make small changes to it before it's included in your website. You can **Minimize** it to make it load as fast as possible also with the option to **Remove Comments** on the fly.

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/gears/cw-gears-f6.png">![Figure-6](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/gears/cw-gears-f6.png "Figure-6"){.uk-thumbnail .uk-thumbnail-mini}</a>

### <a name="opt-cache"></a>Cache

This section gives you more control over the native Joomla cache system by controlling when it is specifically used to help stop conflicts with thing such as forms.
If you choose the turn **Cache Off** option you will also have to define rules for the system to know where to turn the Cache off. To create a new rule add a line consisting of a list of URL parameters for each rule. *\[Figure 7\]*

For example:

    option=com_content&amp;view=article 

Would turn off caching for **com_content** article view. You can also use the **?** as a type of wildcard for example: 
    
    option=com_content&amp;view=article&amp;id=?

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/gears/cw-gears-f7.png">![Figure-7](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/gears/cw-gears-f7.png "Figure-7"){.uk-thumbnail .uk-thumbnail-mini}</a>

### <a name="opt-assets"></a>Assets

The CoalaWeb Gears plugin takes care of the loading of certain assets such as CoalaWeb's custom UIkit and Facebook JS. The requests are stored in a database table with the URL, time and what assets are needed. 

There are two options in this section related to keeping the database clean of old records. The first is to turn on or off the **Auto DB Clean** system which will take care of removing old records. The second is the amount of time that has to elapse before an asset is removed from the database. *\[Figure 8\]*

<div class="uk-alert">Ref: The Lock Time is in minutes and the default value of 1440 min = 1 day.</div> 

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/gears/cw-gears-f8.png">![Figure-8](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/gears/cw-gears-f8.png "Figure-8"){.uk-thumbnail .uk-thumbnail-mini}</a>

### <a name="opt-updates"></a>Updates

<div class="uk-alert">This option is for CoalaWeb Pro extensions that don't come packaged with a <em>Component</em>.</div>

To install the latest **Pro** versions through the Joomla updater you will need to enter your **Download ID** in this section. If you install any additional CoalaWeb Pro extension that don't come packaged with a component you will need to **open and save** the **CW Gears** plugin options again to allow the settings to catch up and be applied to the new extension. *\[Figure 11\]*

<div class="uk-alert">TIP: To stop any typos I recommend copying and pasting the Download ID and also to check for no spaces at the end.</div>

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/gears/cw-gears-f11.png">![Figure-11](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/gears/cw-gears-f11.png "Figure-11"){.uk-thumbnail .uk-thumbnail-mini}</a>

#### <a name="opt-downloadid"></a> Where can I find my Download ID?

To see your **Download ID** you will need to log into [coalaweb.com](https://coalaweb.com) and then go to:

    Members -> My Subscriptions

You will then see the **ID** displayed in the module titled **Download ID**. *\[Figure-11a\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/general/updates/cw-updates-download-id.png">![Figure-11a](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/general/updates/cw-updates-download-id.png "Figure-11a"){.uk-thumbnail .uk-thumbnail-mini}</a>

<div class="uk-alert">TIP: To stop any typos I recommend copying and pasting the download ID and also to check for no spaces at the end.</div>


## <a name="more-help"></a>Need More Help

<div class="uk-alert">Do you have a question that wasn't covered by this GUIDE? Then it's time to drop by the <a href="https://coalaweb.com/forum/index" target="_self">Forum</a></div>