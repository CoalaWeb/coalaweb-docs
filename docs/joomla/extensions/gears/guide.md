## Table of Contents
1.  [Options](#options)
    -   [General](#opt-general)
    -   [jQuery](#opt-jquery)
    -   [Async](#opt-async)
    -   [Uikit](#opt-uikit)
    -   [Custom CSS](#opt-css)
    -   [Custom JS](#opt-js)
    -   [Cache Control](#opt-cache)
4.  [Need More Help?](#more-help)

The CoalaWeb Gears module has a long list of options so we have broken them up into 7 sections which are explained in detail below.

## <a name="options"></a>Options

### <a name="opt-general"></a>General

In the **General** section you have three option the first helps when using **Zoo** by YooTheme by expanding the editor window, making it easier to work on your content. The second option will display a demo of what your system messages will look like, which is great for customizing their style and layout. 

The last option **Gzip help** is designed to help with a know issue where Facebook is unable to access some Joomla sites while using Gzip compression. Not to go into to much detail but it has to do with Facebook only looking at a certain amount of a page and it is misinterpreting some Gzipped sites as being too large. If you turn this option on it will try to detect Facebook and Linking bots and disable Gzip for the duration of their visit. *\[Figure 1\]*

![Figure-1](http://cdn.coalaweb.com/images/docs/joomla-extensions/gears/cw-gears-f1.png "Figure-1"){.coalaweb-docs}

### <a name="opt-jquery"></a>jQuery

This section is designed to help you safely included jQuery on your site with a few cool features. You can choose to load a local copy or from a remote location such as Google's CDN. You can choose which version to included and also if you want **No Conflict** and or **Migrate** turned on. *\[Figure 2\]*

![Figure-2](http://cdn.coalaweb.com/images/docs/joomla-extensions/gears/cw-gears-f2.png "Figure-2"){.coalaweb-docs}

### <a name="opt-async"></a>Async

**Why use async?**
> What you are trying to prevent with the async attribute is parser blocking. If you use the async attribute, you are saying: I don't want the browser to stop what it's doing while it's downloading this script. I know that this script doesn't really depend on anything being ready in the DOM when it runs and it also doesn't need to be run in any particular order.

**Why user defer?**
> Basically, defer tells the browser to wait "until it's ready" before executing the JavaScript in that script block. Usually this is after the DOM has finished loading.

In this section you can decided if you want to add **Asnyc** and or **Defer** to your scripts including an input box to choose which scripts should be included. *\[Figure 3\]*

![Figure-3](http://cdn.coalaweb.com/images/docs/joomla-extensions/gears/cw-gears-f3.png "Figure-3"){.coalaweb-docs}

### <a name="opt-uikit"></a>Uikit

In this section you have the option to turn on a CoalaWeb specific version of Uikit by YooTheme including an option to choose which of the default themes to use. *\[Figure 4\]*

<div class="uk-alert">This option is only going to apply to a select group of CoalaWeb extensions. Unless otherwise asked to I recommend leaving this option set to <em>Yes</em> to ensure certain CoalaWeb extensions function correctly.</div>

![Figure-4](http://cdn.coalaweb.com/images/docs/joomla-extensions/gears/cw-gears-f4.png "Figure-4"){.coalaweb-docs}

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

![Figure-5](http://cdn.coalaweb.com/images/docs/joomla-extensions/gears/cw-gears-f5.png "Figure-5"){.coalaweb-docs}

### <a name="opt-js"></a>Custom JS

In this section you have the option to add custom JS to your website which is great for testing and small tweaks. *\[Figure 6\]*

You can choose to include code added to the **Custom Code** input field and then you have a few options to make small changes to it before it's included in your website. You can **Minimize** it to make it load as fast as possible also with the option to **Remove Comments** on the fly.

![Figure-6](http://cdn.coalaweb.com/images/docs/joomla-extensions/gears/cw-gears-f6.png "Figure-6"){.coalaweb-docs}

### <a name="opt-cache"></a>Cache

This section gives you more control over the native Joomla cache system by controlling when it is specifically used to help stop conflicts with thing such as forms.
If you choose the turn **Cache Off** option you will also have to define rules for the system to know where to turn the Cache off. To create a new rule add a line consisting of a list of URL parameters for each rule. For example:

    option=com_content&amp;view=article 

Would turn off caching for **com_content** article view. You can also use the **?** as a type of wildcard for example: 
    
    option=com_content&amp;view=article&amp;id=?

![Figure-6](http://cdn.coalaweb.com/images/docs/joomla-extensions/gears/cw-gears-f6.png "Figure-6"){.coalaweb-docs}

## <a name="more-help"></a>Need More Help

<div class="uk-alert">Do you have a question that wasn't covered by this GUIDE? Then it's time to drop by the <a href="http://coalaweb.com/forum/index" target="_self">Forum</a></div>