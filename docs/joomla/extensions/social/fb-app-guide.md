## Table of Contents
1.  [Intro](#intro)
2.  [Register and Configure App](#register)
3.  [Extra Security](#extra)
4.  [Need More Help?](#more-help)

## <a class="doc-top" name="intro"></a>Intro

I have tried to maintain a step by step guide on how to create a Facebook App but due to the constant stream of changes Facebook keeps making to their interface I have decided it's best if users consult the guide provided by Facebook. Their guide will always contains the most up to date information. 

<div class="uk-alert">While working your way through their guide I recommend returning here to get tips and help with what settings to choose.</div>

## <a name="register"></a>Register and Configure an App

To get start click <a href="https://developers.facebook.com/docs/apps/register" target="_blank">Here</a> and follow along with the guide consulting the tips below when needed. 

<div class="uk-alert">Note: If you are only using Facebook to manage pages, these instructions will not work you will need a personal Facebook account to continue.</div>

### Tips

When you are creating your Facebook App use the setting below where applicable. *\[Figure-1\]*

- **Platform** Website
- **Namespace** Leave Blank
- **Category** Choose **Utilities**
- **App Domains** Enter your website domain i.e where the extension is installed leaving out the **http**. 
- **Site URL** Enter your website domain i.e where the extension is installed including the **http**. 

<div class="uk-alert">Use the top level domain in the App Domains and Site URL options then you can also use it for sub domains.</div>

![Figure-1](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/social-links/fb-app/cw-fbapp-figure-1.png "Figure-1"){.coalaweb-docs}

You can now copy your **App ID** and paste it into the Facebook App ID field under the **General** tab in the CoalaWeb Social Links component settings. *\[Figure-2\]*

![Figure-2](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/social-links/fb-app/cw-fbapp-figure-2.png "Figure-2"){.coalaweb-docs}

If you are CoalaWeb Social Links Pro subscriber and you want to get Facebook counts using the inbuilt count system you can also add your new Facebook **App ID** and **Secret** to the Facebook options under the **Counts** tab. *\[Figure-3\]*

![Figure-3](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/social-links/fb-app/cw-fbapp-figure-3.png "Figure-3"){.coalaweb-docs}

## <a name="extra"></a>Extra Security

The **Extra Security** setting in the CoalaWeb Social Links Pro count system uses a security feature provided by Facebook to help stop hijacking of the App token and is called **App Secret Proof**. The **App Secret Proof** feature is disabled by default when you create a new **App**. To enable it for your App you will need to go to your App dashboard and do the following. *\[Figure-4\]*

- In the column on the left click on **Settings**.
- Click on the **Advanced** tab.
- Scroll down to the **Security** section.
- Find the toggle for **App Secret Proof** for Server API calls and click it to enable it.

![Figure-4](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/social-links/fb-app/cw-fbapp-figure-4.png "Figure-4"){.coalaweb-docs}

Now that the Facebook App is ready you can head back to the Social Links component options and turn on **FB Extra Security** under the **Counts** tab. *\[Figure-5\]*

![Figure-5](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/social-links/fb-app/cw-fbapp-figure-5.png "Figure-5"){.coalaweb-docs}

## <a name="more-help"></a>Need More Help

<div class="uk-alert">Do you have a question that wasn't covered by this GUIDE? Try the <a href="http://coalaweb.com/support/documentation/category/social-links" target="_self">FAQ</a></div>

<div class="uk-alert">Do you have a question that wasn't covered by this GUIDE or the FAQ? Then it's time to drop by the <a href="http://coalaweb.com/forum/index" target="_self">Forum</a></div>