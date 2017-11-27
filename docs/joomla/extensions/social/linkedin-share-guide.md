## Table of Contents
1.  [Intro](#intro)
2.  [Reachable by LinkedIn](#reachable)
3.  [Open Graph](#og)
    - [Pro Subscribers](#og-pro)
    - [Core Users](#og-core)
    - [Check Open Graph](#og-check)
4.  [Quick Tips](#tips)
5.  [Need More Help?](#more-help)

## <a class="doc-top" name="intro"></a>Intro

**Having problems trying to get LinkedIn to share the correct information?**

I get a lot of questions about how and what gets shared when a LinkedIn button gets clicked so I thought I would put together a check list to make sure you are getting the most out of your share buttons.

## <a name="reachable"></a>Reachable by LinkedIn

**Is your website online and accessible to the public?**

The first thing you need to understand is if LinkedIn can't reach your page then it has no way of retrieving and storing the information needed. This leads me to the very important question, is your website live and is it reachable by the public? If your site is offline for development or maintenance then the LinkedIn bots can't reach your site thus have no way of creating a record of your page.

## <a name="og"></a>Open Graph

**Tip:** LinkedIn stores image information for up to 7 days so any image changes you make or if you have just brought your site back online can take up to 7 days to catch up.

To make sure what LinkedIn shares is as accurate as possible you will need to include **Open Graph** meta tags in the head of each of your pages you have a share button published on. They typically included the follow tags:

-   og:title
-   og:image
-   og:url
-   og:description

### <a name="og-pro"></a>CoalaWeb Pro Subscribers

For CoalaWeb Social Links Pro subscribers you will already have a plugin to take care of adding all of this info for your automatically based on the page details. To learn more check out this [Guide Link](https://coalaweb.com/support/documentation/item/coalaweb-social-links-guide#options-og) 

The main thing you will need to ensure is that it is turned on so open up the CoalaWeb Social Links **Component Options** and make sure that under the **Metadata Plugin** tab in the **Facebook Only** section the **Add Open Graph** option is set to **Yes**

### <a name="og-core"></a>CoalaWeb Core Users

There are loads of free Open Graph plugins over in [JED](https://extensions.joomla.org/extensions/extension/?searchall=Open+Graph&filter%5Btags%5D%5B%5D=&filter%5Bcore_catid%5D=&filter%5Bincludes%5D=&filter%5Bversions%5D=&filter%5Btype%5D=free&filter%5Bhasdemo%5D=&order=&filter%5Bnewupdated%5D=&filter%5Bscore%5D=&filter%5Bfavourites%5D=&dir=DESC&limitstart=0&controller=filter&view=extension&layout=list&Itemid=145&clearorders=0&clearfilters=1) so have a look around to see if one fits your needs.

### <a name="og-check"></a>Check Open Graph Tags

To check that the Open Graph tags are being included start by opening up one of your articles then right click the page and finally select **View Page Source** If all has gone according to plan you should see something like this in the head of the page. *\[Figure-3\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/social-links/fb-share/cw-fbshare-figure3.png">![Figure-3](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/social-links/fb-share/cw-fbshare-figure3.png "Figure-3"){.uk-thumbnail .uk-thumbnail-mini}</a>

**How do I update what LinkedIn has stored?**

1. If your site doesn't have any errors and LinkedIn can see and retrieved your page information you can wait up to 7days for your pages to automatically catch up.

2. The only manual way to **clear** the sharing preview **cache** for LinkedIn is to trick LinkedIn into thinking your page is different. This can be done by adding a dummy parameter to the page URL. It won't affect your webpage, but it does force the metadata to be re-fetched. So if the URL is **http://example.com/sample.html**, you could use **http://example.com/sample.html?doNothing=1** then once you have refreshed the page try your share button again.

## <a name="tips"></a>Quick Tips

1. Here are the image requirements specific to the LinkedIn sharing module:

    - Max file size: 5 MB
    - Minimum image dimensions: 1200 (w) x 627 (h) pixels
    - Recommended ratio: 1.91:1

    Note: If the image meets the requirements, but it still does not appear in updates on LinkedIn, your website may be blocking us from pulling the image or the image may be located on a protected directory or website.

2. LinkedIn stores page information for up to 7 days so any changes you make or if you have just brought your site online can take up to 7 days to catch up.

3. Stubborn pages, if you find the majority of your pages are displaying correctly but a particular page isn't try using the dummy parameter option metioned above to force it to catch up. Once you have refreshed the page test your button again.

4. LinkedIn Guide: [Making Your Website Shareable on LinkedIn](https://www.linkedin.com/help/linkedin/answer/46687/making-your-website-shareable-on-linkedin) 

## <a name="more-help"></a>Need More Help

<div class="uk-alert">Do you have a question that wasn't covered by this GUIDE? Try the <a href="https://coalaweb.com/support/documentation/category/social-links" target="_self">FAQ</a></div>

<div class="uk-alert">Do you have a question that wasn't covered by this GUIDE or the FAQ? Then it's time to drop by the <a href="https://coalaweb.com/forum/index" target="_self">Forum</a></div>