## Table of Contents
1.  [Intro](#intro)
2.  [App Background](#background)
    - [Is an App compulsory?](#bg-compulsory)
	- [Where, why and how is it used?](#bg-how)
3.  [App Creation](#creation)
    - [Overview](#creation-overview)
    - [Register and Configure App](#register)
    - [Extra Security](#extra)
    - [Do I need a review?](#review)
4.  [Privacy Policy](#privacy)
     - [Overview](#privacy-overview)
     - [Privacy Policy Example](#privacy-example)
     - [Disclaimer](#privacy-disclaimer)
     - [Acknowledgments](#privacy-acknowledge)
4.  [Need More Help?](#more-help)

<div class="uk-alert uk-alert-warning"><i class="uk-icon-calendar"></i> Last updated on the 15th of May 2018</div>

## <a class="doc-top" name="intro"></a>Intro

Facebook has made some changes recently to their App system such as a few settings that were once optional are now compulsory plus the inclusion of a new warning message titled: App Review required by August 1, 2018 to retain access to Facebook Platform APIs

## <a name="background"></a>App Background

Before you get started creating a Facebook App let me explain a bit about what it is and how it's used by CoalaWeb Social Links.

### <a name="bg-compulsory"></a>Is an App compulsory?

The short answer is **No**. The long answer is that the CoalWeb Social Links extension uses a Facebook App to enhance the system but it isn't necessary for it to function correctly. 

### <a name="bg-how"></a>Where, why and how is it used?

The App ID is added to a page through the CoalaWeb Facebook JS plugin and or included in an Open Graph tag and or used to check a page's social counts. It is used by CoalaWeb Social Links in the following ways:

#### Core and Pro users
- The newer based sharing button. You can use the older sharing system which doesn't need an APP ID by selecting it in the component general options
- Loading of the CoalaWeb Page module. The module will display correclty without an App ID.

#### Pro Users
- Used with Open Graph tags to help with insights. The Open Graph system will work fine without an App ID
- The App ID and App Secret can be used when retrieving the current Share, Comment and Total Facebook counts for a page. Version 1.0.0+ will work with out n App.

<div class="uk-alert">Note: With the release of version <strong>1.0.0</strong> of CoalaWeb Social Links the count system will work without the use an App. On large sites that make a lot of API requests I recommend setting a large <strong>locktime</strong> and potentially adding an App ID and App Secret through the component options to increase the API limit.</div>

## <a name="creation"></a>App Creation

If you have decided you want to create a Facebook App and use it with the CoalaWeb Social Links extension read on.

### <a name="creation-overview"></a>Overview

I have tried to maintain a step by step guide on how to create a Facebook App but due to the constant stream of changes Facebook keeps making to their interface I have decided it's best if users consult the guide provided by Facebook. Their guide will always contains the most up to date information. 

<div class="uk-alert">While working your way through their guide I recommend returning here to get tips and help with what settings to choose.</div>

### <a name="register"></a>Register and Configure an App

To get start click <a href="https://developers.facebook.com/docs/apps/register" target="_blank">Here</a> and follow along with the guide consulting the tips below when needed. 

<div class="uk-alert">Note: If you are only using Facebook to manage pages, these instructions will not work you will need a personal Facebook account to continue.</div>

#### Tips

When you are creating your Facebook App use the setting below where applicable. *\[Figure-1\]*

- **Platform** Website
- **Namespace** Leave Blank
- **Category** Choose **Utilities**
- **App Domains** Enter your website domain i.e where the extension is installed leaving out the **http**. 
- **Privacy Policy URL** You must provide a Privacy Policy URL. Must be provided to take your app public.
- **Terms of Service URL** You must provide a Terms of Service URL.
- **Site URL** Enter your website domain i.e where the extension is installed including the **http**.
- **Privacy Policy URL** - You must provide a Privacy Policy URL. Must be provided to take your app public.
- **Terms of Service URL** - You must provide a Terms of Service URL.

<div class="uk-alert">Use the top level domain in the App Domains and Site URL options then you can also use it for sub domains.</div>

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/social-links/fb-app/cw-fbapp-figure-1.png">![Figure-1](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/social-links/fb-app/cw-fbapp-figure-1.png "Figure-1"){.uk-thumbnail .uk-thumbnail-mini}</a>


You can now copy your **App ID** and paste it into the Facebook App ID field under the **General** tab in the CoalaWeb Social Links component settings. *\[Figure-2\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/social-links/fb-app/cw-fbapp-figure-2.png">![Figure-2](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/social-links/fb-app/cw-fbapp-figure-2.png "Figure-2"){.uk-thumbnail .uk-thumbnail-mini}</a>

If you are CoalaWeb Social Links Pro subscriber and you want to get Facebook counts using the inbuilt count system you can also add your new Facebook **App ID** and **Secret** to the Facebook options under the **Counts** tab. *\[Figure-3\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/social-links/fb-app/cw-fbapp-figure-3.png">![Figure-3](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/social-links/fb-app/cw-fbapp-figure-3.png "Figure-3"){.uk-thumbnail .uk-thumbnail-mini}</a>

### <a name="extra"></a>Extra Security

The **Extra Security** setting in the CoalaWeb Social Links Pro count system uses a security feature provided by Facebook to help stop hijacking of the App token and is called **App Secret Proof**. The **App Secret Proof** feature is disabled by default when you create a new **App**. To enable it for your App you will need to go to your App dashboard and do the following. *\[Figure-4\]*

- In the column on the left click on **Settings**.
- Click on the **Advanced** tab.
- Scroll down to the **Security** section.
- Find the toggle for **App Secret Proof** for Server API calls and click it to enable it.

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/social-links/fb-app/cw-fbapp-figure-4.png">![Figure-4](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/social-links/fb-app/cw-fbapp-figure-4.png "Figure-4"){.uk-thumbnail .uk-thumbnail-mini}</a>

Now that the Facebook App is ready you can head back to the Social Links component options and turn on **FB Extra Security** under the **Counts** tab. *\[Figure-5\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/social-links/fb-app/cw-fbapp-figure-5.png">![Figure-5](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/social-links/fb-app/cw-fbapp-figure-5.png "Figure-5"){.uk-thumbnail .uk-thumbnail-mini}</a>

### <a name="review"></a>Do I need a review?

Recently a new message has appeared in the App adminstation window titled:
 
> App Review required by August 1, 2018 to retain access to Facebook Platform APIs

As far as I'm aware none of the situations mentioned in the [Where, why and how](#bg-how) section require an App review as outlined by Facebook:

> If your app uses advanced FB Login or Messenger permissions, or if you want your app to be listed in App Center, you need to submit the app for review.

<div class="uk-alert">Based on my research Apps should continue to function for the purposes of the CoalaWeb Social Links extension after the 1st of August even with no review.</div>

## <a name="privacy"></a>Privacy Policy

Facebook has recently made the Privacy Policy and Terms of Service URLs compulsory for all Apps so if you have created and App or you are looking to update an existing one read on.

> Privacy Policy URL - You must provide a Privacy Policy URL. Must be provided to take your app public.
> Terms of Service URL - You must provide a Terms of Service URL.

### <a name="privacy-overview"></a>Overview

In most cases a Joomla based website should already have these two documents but I have included a basic Privacy Policy template that can be used as a stand alone privacy policy or can be integrated into an already existing one.

### <a name="privacy-example"></a>Privacy Policy Example

Privacy and data protection example policy

You may visit our website without providing personal details. Your personal details will only be collected if you freely disclose them during your visit to our website.

Our website contains programmes (plug-ins) operated by the social network Facebook. These programmes are exclusively operated by Facebook Inc., 1601 S. California Ave, Palo Alto, CA 94304 USA (Facebook). The plug-ins are clearly visible on our website through the use of the Facebook logo or through the add-on “like” and or "Share" buttons.

When visiting our website containing such a plug-in, your browser will establish a direct link with the servers operated by Facebook; as a result the content of the plug-in will be transferred to your browser and embedded in the website being shown.

If you visit our website whilst signed into your Facebook user account, information concerning your visit will be transferred to Facebook. Facebook can assign your visit to our website and to your user account. Information arising from interaction with a Facebook plug-in (such as by clicking a Facebook “like” button) will be directly transferred to and stored by Facebook. To prevent this you must log out of your Facebook account before visiting our website.

Please refer to Facebook’s privacy policy, also known as it's “Data Use Policy.” (https://www.facebook.com/full_data_use_policy) for more information on: the purpose and scope of data collection and data analysis undertaken by Facebook, your rights, how to modify settings and how to protect your privacy.

If you have any questions about data collection, analysis and use of personal data, disclosure, amendment, blocking and deletion of personal data contact: (Name and address of contact for data protection or data protection ombudsman)

### <a name="privacy-disclaimer"></a>Disclaimer

Please be advised: the true extent of the way in which Facebook uses the data it receives is unknown. As a result it is not possible to produce a privacy policy statement which satisfies every legal eventuality. CoalaWeb therefore accepts no liability for third party claims arising either directly or indirectly as a result of the use of the privacy policy template example above.

### <a name="privacy-acknowledge"></a>Acknowledgments

## <a name="more-help"></a>Need More Help

<div class="uk-alert">Do you have a question that wasn't covered by this GUIDE? Try the <a href="https://coalaweb.com/support/documentation/category/social-links" target="_self">FAQ</a></div>

<div class="uk-alert">Do you have a question that wasn't covered by this GUIDE or the FAQ? Then it's time to drop by the <a href="https://coalaweb.com/forum/index" target="_self">Forum</a></div>