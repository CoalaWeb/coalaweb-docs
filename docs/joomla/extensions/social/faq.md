## List of Questions
1.  [Can I install CoalaWeb Social Links on multiple domains?](#q1)
2.  [Can I keep using CoalaWeb Social Links when my subscription runs out?](#q2)
3.  [Can I remove the Powered by CoalaWeb from the module?](#q3)
4.  [Can I change the images used in module?](#q4)
5.  [I'm having problems validating my webiste with W3C what can I do?](#q5)
6.  [Facebook error - Given URL is not allowed by the Application](#q6)
7.  [My custom Follow Us image isn't displaying correctly?](#q7)
8.  [I'm using a RocketTheme template and the Tabs module isn't displaying?](#q8)
9.  [The CoalaWeb Meta tab isn't displaying in my article editor?](#q9)
10. [Why did my Likebox disappear after updating to version 0.2.5?](#q10)
11. [I'm using a JA T3 template and the Tabs module isn't displaying?](#q11)
12. [Wrong image and or information is being shared?](#q12)
13. [How to display Tabs module when using JA Builder?](#q13)
14. [Lost my Facebook feed in Page module after upgrade to 0.4.2?](#q14)
15. [Browser inspector error: Load denied by X-Frame-Options?](#q15)

***

#### <a class="doc-top" name="q1"></a>Can I install CoalaWeb Social Links on multiple domains?

**YES** - You can install Social Links on as many domains as you want. There is no domain check or restriction.

***

#### <a name="q2"></a>Can I keep using CoalaWeb Social Links when my subscription runs out?

**YES** - If you have purchased a CoalaWeb PRO subscription, you have access to PRO downloads, updates and support for the length of the subscription. After it has run out you can keep using the version you have installed. However, you will no longer be able to update to a newer versions or receive support. Of course you can renew your subscription to gain access again or you can choose to downgrade to the FREE version its up to you.

***

#### <a name="q3"></a>Can I remove the Powered by CoalaWeb from the module?

**YES** - You can turn the link off in the Free or Pro versions by opening up the module configuration and its under **Advanced Options -> Display link to author**.

***

#### <a name="q4"></a>Can I change the images used in module?

**YES** - Creating a theme is easy, just copy the custom-example folder found in:

    media → coalawebsocial → components → sociallinks → themes-icon

Give the theme a different name, edit the files as needed and of course add your custom icons. All the folders located in the themes-icon directory will automatically be listed in the Icon Styles select list.

***

#### <a name="q5"></a>I'm having problems validating my webiste with W3C what can I do?

Each social network handles there formatting differently but the majority of them are now pushing towards HTML5 but below I have included some exceptions and know issues.

#### Joomla using HTML5

**Linkedin:**

> The text content of element script was not in the required format: Expected space, tab, newline, or slash but found l instead.

This is due to Linkedin placing a language reference such as this lang:en_GB inside the script tags.

**Stumbleupon:**

> Element name su:badge cannot be represented as XML 1.0. Element su:badge not allowed as child of element div in this context. (Suppressing further errors from this subtree.)

This is due to StumbleUpon not support HTML 5 as of yet I have included a link below outining this issue.
[StumbleUpon and HTML5](https://getsatisfaction.com/stumbleupon_help_center/topics/stumbleupon_button_does_not_validate_for_html5_w3c)

#### Joomla using XHTML 1.0 Transitional

> There is no attribute X

Any data attributes such as data-href wont pass as they are designed for HTML5 but they work fine just be aware

Now StumbleUpon will cause the following errors:

*   element "su:badge"
*   undefined there is no attribute "location"
*   there is no attribute "layout"

These won’t affect the functionality of the button but I have yet to find a solid solution but I will keep looking.

<div class="uk-alert">I will continue to implement changes with each new release as solutions become available.</div>

***

#### <a name="q6"></a>Facebook error - Given URL is not allowed by the Application

The problem is that whatever **URL** you are currently hosting your Application on is not setup in your Application configuration.

**Steps**

1.  Go to **Basic** settings for your app
2.  Select **Add Platform**
3.  Select **Website**
4.  Put your website URL under **Site URL**

You can see more details in Step 9 of this [Guide](https://coalaweb.com/support/documentation/item/create-facebook-application)

***

#### <a name="q7"></a>My custom Follow Us image isn't displaying correctly?

This will normally be for one of two reasons:

1. You have **Spaces** in the **Name** of the image you have selected which is an easy fix just rename your image and then reselect it from the module configuration.

2. You have some strange server configuration so Joomla is miss interpreting the URL of the image. To fix this one just use the **External** image option but make sure to leave the image selector option blank as this overrides the external image option.

***

#### <a name="q8"></a> I'm using a Rocket Theme template and the Tabs module isn't displaying?

Try publishing the **Tabs** module to one of the **utility** positions rather than **debug** for example **utility-a**. Also make sure you have set some of the Tabs to display.

***

#### <a name="q9"></a> The CoalaWeb Meta tab isn't displaying in my article editor?

For the CoalaWeb Meta tab to display correctly in your article editor the **Show Article Options** option needs to be set to **Show**. This option can be found at:

> Articles -> Options -> Editing Layout -> Show Article Options

This is because the Meta options contained in the CoalaWeb tab extend the article options.

***

#### <a name="q10"></a> Why did my Likebox disappear after updating to version 0.2.5?

The CoalaWeb Likebox module was superseded by the Page module in Version 0.2.1 June 2015. Starting with version 0.2.5 the obsolete CoalaWeb Likebox module is no longer packaged with the Social Links extension and or supported so please if you haven’t already started using the CoalaWeb Page module you will need to start as of version 0.2.5.

***

#### <a name="q11"></a> I'm using a JA T3 template and the Tabs module isn't displaying?

In newer JA T3 templates the Debug module position exists but you have to assign it to a location.

##### For example:

- Open up your JA template options (I'm using the T3 BS3 Blank template) and choose the **Layout** tab from the top.
- Next scroll down to the **Footer** positions and select **6** from the footer **pagination** so you can see footer-6 (to make sure it's not being used).
- Next click the **gear** icon in the **top right** corner then click in the **Select a Position** box and then **Debug** from the list.  *\[Figure-1\]*
- Lastly **Save** your template settings and the debug position should now display as expected.

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/social-links/faq/cw-social-links-faq-f1.png">![Figure1](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/social-links/faq/cw-social-links-faq-f1.png "Figure-1"){.uk-thumbnail .uk-thumbnail-mini}</a>

***

#### <a name="q12"></a> Wrong image and or information is being shared?

<div class="uk-alert">Are you using the <strong>Free (Core)</strong> version or the <strong>Pro</strong> version of CoalaWeb Social Links?</div>

The **Pro** version comes with a meta tags system that auto generates **Open Graph**, **Twitter Card** and **Schema** tags which can also be overridden on a per item basis - [Read More](https://coalaweb.com/support/documentation/item/coalaweb-social-links-guide).

If you are using the **Core** version no problem there are loads of free **Open Graph** extension over on **JED** [Here](https://extensions.joomla.org/extensions/extension?searchall=open+graph&filter%5Btags%5D%5B%5D=&filter%5Bcore_catid%5D=&filter%5Bincludes%5D=&filter%5Bversions%5D=&filter%5Btype%5D=free&filter%5Bhasdemo%5D=&order=&filter%5Bnewupdated%5D=&filter%5Bscore%5D=&filter%5Bfavourites%5D=&dir=DESC&limitstart=0&controller=filter&view=extension&layout=list&Itemid=145&clearorders=0&clearfilters=1) is a link filtered for free Open Graph extensions.

<div class="uk-alert">To understand more about the sharing system I have also written a <a href="https://coalaweb.com/support/documentation/item/coalaweb-docs-facebook-sharing-guide">Guide</a> with tips and info on the subject.</div>

##### Quick Tips:

> If the image referenced by the Open Graph tags is too small Facebook will move onto another image that it finds on the page that meets the minimum size restrictions. FB will only use images that are at least 200 x 200px and prefers images that are measured in multiples of 100 and are in a square format.

> Facebook stores page information for up to 24 hours so any changes you make or if you have just brought your site online can take up to 24 hours to catch up.

***

#### <a name="q13"></a> How to display Tabs module when using JA Builder?

Here is a work around to get Social Tabs displaying on a site built with JA Builder.

- Open up a page in the JA Builder editor
- Add a block to the **Footer**
- Choose type **Spotlight**
- A 6-6 layout is fine (we will only be using one)
- Click **Select Widget** (either one is fine) and then **Settings** (cog icon)
    - Content type = **Module**
    - Module = **Social Tabs**
    - Style = **None**

Then from the side of the block select the **Settings** (cog icon) for the entire block.

- Container = **fluid**
- Padding = **None**

Then **Publish** the page and you should now have a hidden module position and the Social Tabs should be displaying as expected. The footer is display on all the pages so you should only have to add it once.

***

#### <a name="q14"></a> Lost my Facebook feed in Page module after upgrade to 0.4.2?

##### Background

Facebook has depreciated the **Post** option and replaced it with **Tabs** which allows users to display a series of tabs such as **Timeline**, **Messages** and or **Events** with in the **Page** module.

##### Fix

As of Social Links version **0.4.2** the old system has been replaced by **Tabs** which is a multi select field where you will need to choose one or more of the tabs that you want to be displayed.

<div class="uk-alert">Note: This field can be left blank for users who don't want to display any tabs.</div>

***

#### <a name="q15"></a> Browser inspector error: Load denied by X-Frame-Options?

While using the **CoalaWeb Page** module with the **Timeline** displayed you may have seen this error being displayed in the browser inspector.

##### Background

> The **X-Frame-Options** HTTP response header can be used to indicate whether or not a browser should be allowed to  render a page in a \<frame>, \<iframe> or \<object> . Sites can use this to avoid clickjacking attacks, by ensuring that their content is not embedded into other sites.

So basically when the **Timeline** is feed into the **Page** module some parts are held back due to the settings on the Facebook site. The module and it's content will continue to be displayed as expected this is just a warning that some of it's content is not displayed due to X-Frame-Options.

<div class="uk-alert">Note: This error will display even if you generate code from the <a href="https://developers.facebook.com/docs/plugins/page-plugin/" target="_blank">Facebook Page Plugin</a> page and paste it into your site.</div>

##### Fix

Firstly the module content will continue to be displayed as expected so you can feel free to leave it as is. If you want to stop this warning from displaying the only option currently is to turn off the **Timeline** by removing it from the **Tabs** module option.

##### Extra Info

I will continue to follow this up with the Facebook developers and update this FAQ with any new info I get but if anyone else has extra info on the subject please [Contact Me](https://coalaweb.com/support/get-in-touch/contact-us).

***