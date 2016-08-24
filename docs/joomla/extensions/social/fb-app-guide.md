## Table of Contents
1.  [Intro](#intro)
1.  [Register and Configure App](#register)
1.  [Get App Token](#token)
2.  [Extra Security](#extra)
3.  [Need More Help?](#more-help)

## <a class="doc-top" name="intro"></a>Intro

I have tried to maintain a step by step guide on how to create a Facebook App but due to the constant stream of changes Facebook keeps making to the interface I have decided it's best if users consult the guide provided by Facebook. Their guide will always contains the most up to date information. 

<div class="uk-alert">While working your way through their guide I recommend returning here to get tips and help with what settings to choose.</div>

## <a name="register"></a>Register and Configure an App

To get start click [Here](https://developers.facebook.com/docs/apps/register) and follow along with the guide provided by Facebook consulting the tips below when needed. 

<div class="uk-alert">Note: If you are only using Facebook to manage pages, these instructions will not work you will need a personal Facebook account to continue.</div>

### Tips

When you are creating your Facebook App use the setting below where applicable. *\[Figure-1\]*

**Platform** Website
**Namespace** Leave Blank
**Category** Choose **Utilities**
**App Domains** Enter your website domain i.e where the extension is installed leaving out the **http**. 
**Site URL** Enter your website domain i.e where the extension is installed including the **http**. 

<div class="uk-alert">Use the top level domain in the App Domains and Site URL options then you can also use it for sub domains.</div>

![Figure-1](http://cdn.coalaweb.com/images/docs/joomla-extensions/social-links/fb-app/cw-fbapp-figure-1.png "Figure-1"){.coalaweb-docs}

You can now copy your **App ID** and paste it into the CoalaWeb extension settings. *\[Figure-2\]*

![Figure-2](http://cdn.coalaweb.com/images/docs/joomla-extensions/social-links/fb-app/cw-fbapp-figure-2.png "Figure-2"){.coalaweb-docs}

## <a name="token"></a>Get App Token

If you want to retrieve and store a page's count using the CoalaWeb Social Links Pro inbuilt count system you will need create a **Facebook App** and use it's **App ID** and **App Secret** to generate an **App Access** Token. 

To create an App Access Token click this [link](https://smashballoon.com/custom-facebook-feed/access-token/) and scroll down to the bottom of the page and enter Your **App ID** and **App Secret** into the input fields and then click **Get my Access Token** once it has finished note down the generated App Access Token ready to be used in CoalaWeb extension settings. *\[Figure-3\]*

![Figure-3](http://cdn.coalaweb.com/images/docs/joomla-extensions/social-links/fb-app/cw-fbapp-figure-3.png "Figure-3"){.coalaweb-docs}

## <a name="token"></a>Extra Security

The **Extra Security** setting in the CoalaWeb Social Links Pro count system uses a security feature provided by Facebook to stop hijacking of the App token which is called **App Secret Proof**. The **App Secret Proof** feature is disabled by default when you create a new **App**. To enable it for your app you will need to go to your app dashboard and do the following. *\[Figure-4\]*

    In the column on the left click on **Settings**.
    Click on the **Advanced** tab.
    Scroll down to the **Security** section.
    Find the toggle for **App Secret Proof** for Server API calls and click it to enable it.

![Figure-4](http://cdn.coalaweb.com/images/docs/joomla-extensions/social-links/fb-app/cw-fbapp-figure-4.png "Figure-4"){.coalaweb-docs}

Now that the Facebook App is ready you can head back to the Social Links component options, turn on the **FB Extra Security** option and enter your **App Secret** into the **FB App Secret** field. *\[Figure-5\]*

![Figure-5](http://cdn.coalaweb.com/images/docs/joomla-extensions/social-links/fb-app/cw-fbapp-figure-5.png "Figure-5"){.coalaweb-docs}

## <a name="more-help"></a>Need More Help

<div class="uk-alert">Do you have a question that wasn't covered by this GUIDE? Try the <a href="http://coalaweb.com/support/documentation/category/social-links" target="_self">FAQ</a></div>

<div class="uk-alert">Do you have a question that wasn't covered by this GUIDE or the FAQ? Then it's time to drop by the <a href="http://coalaweb.com/forum/index" target="_self">Forum</a></div>