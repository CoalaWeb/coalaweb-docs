## Table of Contents
1.  [Overview](#overview)
2.  [Updates](#updates)
    - [Where is my Download ID?](#options-downloadid)
3.  [Options](#options)
4.  [Advanced \[Pro\]](#advanced)
5.  [Need More Help?](#more-help)

## <a class="doc-top" name="overview"></a>Overview

**CoalaWeb Analytics** gives Joomla administrators the power to load the most up to date version of the Google Analytics tracking code. It will be loaded and executed asynchronously on all browsers.

<div class="uk-alert">When installing all the parts of the system will be installed at the same time making installing, upgrading and uninstalling a breeze.</div>

## <a name="updates"></a>Updates

The **CoalaWeb Analytics** extension integrates with the inbuilt **Joomla Update** system so both **Core** and **Pro** users can keep their extension up to date. For **Core** users when you see updates listed in the Joomla update manager feel free to select it and update. 

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

### <a name="options"></a>Options

This section has two options that are available in both the **Core** and **Pro** versions. 

The first one is the **Property ID** (also called the **Tracking ID**) which can be found in your Google Analytics account. If you are not sure where to find it the quickest and easiest way is to follow these steps. *\[Figure-2\]*

    - Sign into your Google analytics account.
    - Click the little graph icon in the top left corner to display the list of accounts.
    - In the list you will see the ID next to the account name.

<div class="uk-alert">Note: Your site will not be tracked unless the <strong>Property ID</strong> is entered.</div>
 
The second option in this section is used if you want to verify that your are the site owner using the **HTML Tag** method. To get the **Content Code** just open up **Webmaster Tools** and then select **Verifications Methods**. Next choose **HTML Tag** from the options and lastly extract **only** the content code from between the inverted commas. Once you have your code set the **Verify** option to **Yes** and paste it into the **Meta Tag Content** field.

Once you have set up the **Content Code** you should be bale to go back to **Webmaster Tools** and verify that you are the website owner.  *\[Figure-2\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/analytics/cw-analytics-f2.png ">![Figure-2a](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/analytics/cw-analytics-f2.png "Figure-2a"){.uk-thumbnail .uk-thumbnail-mini}</a>
              
### <a name="advanced"></a>Advanced \[Pro\]

<div class="uk-alert"><strong>Pro</strong> subscribers also get some advanced option that covered in detail below.</div>

The **Tracking Area** option controls if the analytic code is added to **Site**, **Admin** or **Both** pages. *\[Figure-3\]*

The **Tracking Method** has two options avaliable. The **Standard** method which ensures the script will be loaded and executed asynchronously on all browsers or the **Alternative Async** method which adds support for **preloading** which provides a performance boost on modern browsers. *\[Figure-3\]*

The **Object Name** option is used in cases where you'd like to add analytics code to your website, but the **ga** variable is already being used for something else. In these situations you can change the object name by entering an alternative. *\[Figure-3\]*

<div class="uk-alert">Note: In the majority of cases it's best to leave this option set to <strong>ga</strong>.</div>

In some situation you may need **IP Anonymization** which will anonymize the IP address of the hit sent to Google Analytics. This maybe for example due to local law requirements in these cases you can set this option to **Yes**. *\[Figure-3\]*
  
To make the code snippet easier to identify it is surrounded by following opening and closing tags.
 
    <!-- CoalaWeb Google Analytics --><!-- End CoalaWeb Google Analytics -->
    
If you prefer not to display these tags you can set this option to **No**. *\[Figure-3\]*
  
<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/analytics/cw-analytics-f3.png ">![Figure-3](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/analytics/cw-analytics-f3.png "Figure-3"){.uk-thumbnail .uk-thumbnail-mini}</a>

## <a name="more-help"></a>Need More Help

<div class="uk-alert">Do you have a question that wasn't covered by this GUIDE? Then it's time to drop by the <a href="https://coalaweb.com/forum/index" target="_self">Forum</a></div>