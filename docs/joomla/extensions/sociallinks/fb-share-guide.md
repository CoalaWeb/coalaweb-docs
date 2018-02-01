## Table of Contents
1.  [Intro](#intro)
2.  [Reachable by Facebook](#reachable)
    - [Using Gzip](#gzip)
3.  [Open Graph](#og)
    - [Pro Subscribers](#og-pro)
    - [Core Users](#og-core)
    - [Check Open Graph](#og-check)
    - [Not Using Open Graph](#og-not)
4.  [Open Graph Debug Tool](#debug)
5.  [Quick Tips](#tips)
6.  [Need More Help?](#more-help)

## <a class="doc-top" name="intro"></a>Intro

**Having problems trying to get Facebook to share the correct information?**

I get a lot of questions about how and what gets shared when a Facebook button gets clicked so I thought I would put together a check list to make sure you are getting the most out of your share buttons.

## <a name="reachable"></a>Reachable by Facebook

**Is your website online and accessible to the public?**

The first thing you need to understand is if Facebook can't reach your page then it has no way of retrieving and storing the information needed. This leads me to the very important question, is your website live and is it reachable by the public? If your site is offline for development or maintenance then the Facebook bots can't reach your site thus have no way of creating a record of your page.

### <a name="gzip"></a>Using Gzip

There is a known issue with Joomla 3.+, Gzip and Facebook. It is basically due to Facebook interpreting some pages as being too large when this options is being used and as a consequence returns an error. If you are using a CoalaWeb extension I have added an option to the **System CW Gears** framework plugin (that comes packaged with all my extensions) to fix this issue it basically turns off GZip compression when the Facebook or Linkedin bots visits your page.

To use this option open up your plugin manager and search for **gears**. *\[Figure-1\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/social-links/fb-share/cw-fbshare-figure1.png">![Figure-1](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/social-links/fb-share/cw-fbshare-figure1.png "Figure-1"){.uk-thumbnail .uk-thumbnail-mini}</a>

Then under the **General** tab turn on the **Gzip Help** option and save and close the plugin options. Its always a good idea to clear your Joomla cache after making changes to make sure they catch up. *\[Figure-2\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/social-links/fb-share/cw-fbshare-figure2.png">![Figure-2](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/social-links/fb-share/cw-fbshare-figure2.png "Figure-2"){.uk-thumbnail .uk-thumbnail-mini}</a>

## <a name="og"></a>Open Graph

**Tip:** Facebook stores page information for up to 24 hours so any changes you make or if you have just brought your site back online can take up to 24 hours to catch up.

To make sure what Facebook shares is as accurate as possible you will need to include **Open Graph** meta tags in the head of each of your pages you have a share button published on. They typically included the follow tags:

-   og:title
-   og:type
-   og:image
-   og:url
-   og:site_name
-   og:description

### <a name="og-pro"></a>CoalaWeb Pro Subscribers

For CoalaWeb Social Links Pro subscribers you will already have a plugin to take care of adding all of this info for your automatically based on the page details. To learn more check out this [Guide Link](https://coalaweb.com/support/documentation/item/coalaweb-social-links-guide#options-og) 

The main thing you will need to ensure is that it is turned on so open up the CoalaWeb Social Links **Component Options** and make sure that under the **Metadata Plugin** tab in the **Facebook Only** section the **Add Open Graph** option is set to **Yes**

### <a name="og-core"></a>CoalaWeb Core Users

There are loads of free Open Graph plugins over in [JED](https://extensions.joomla.org/extensions/extension/?searchall=Open+Graph&filter%5Btags%5D%5B%5D=&filter%5Bcore_catid%5D=&filter%5Bincludes%5D=&filter%5Bversions%5D=&filter%5Btype%5D=free&filter%5Bhasdemo%5D=&order=&filter%5Bnewupdated%5D=&filter%5Bscore%5D=&filter%5Bfavourites%5D=&dir=DESC&limitstart=0&controller=filter&view=extension&layout=list&Itemid=145&clearorders=0&clearfilters=1) so have a look around to see if one fits your needs.

### <a name="og-check"></a>Check Open Graph Tags

To check that the Open Graph tags are being included start by opening up one of your articles then right click the page and finally select **View Page Source** If all has gone according to plan you should see something like this in the head of the page. *\[Figure-3\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/social-links/fb-share/cw-fbshare-figure3.png">![Figure-3](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/social-links/fb-share/cw-fbshare-figure3.png "Figure-3"){.uk-thumbnail .uk-thumbnail-mini}</a>

### <a name="og-not"></a>Not using Open Graph

If you aren't using Open Graph tags and your site is reachable by Facebook they will try to retrieve page details as best they can by using such things as normal meta tags and scrapping the page to find usable images.

Can I see what Facebook sees when looking at my website?

## <a name="debug"></a>Open Graph Debug Tool

**Tip:** To use the Debugger Tool you will need to have a Facebook account and be logged in.

Facebook provides a great tool for fault finding issues called the [Debugger](https://developers.facebook.com/tools/debug/) it allows you to quickly and easily identify any issues with a particular web page. To get started enter in the URL of a page you want to check and click **Debug**. *\[Figure-4\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/social-links/fb-share/cw-fbshare-figure4.png">![Figure-4](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/social-links/fb-share/cw-fbshare-figure4.png "Figure-4"){.uk-thumbnail .uk-thumbnail-mini}</a>

On the next page you have a tonne of helpful information but lets start at the top with the title **When and how we last scraped the URL** here you can see if there were any problem reaching your page, the last time it was scrapped and even current **Likes** and **Shares** for that particular page. *\[Figure-5\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/social-links/fb-share/cw-fbshare-figure5.png">![Figure-5](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/social-links/fb-share/cw-fbshare-figure5.png "Figure-5"){.uk-thumbnail .uk-thumbnail-mini}</a>

In the next section you can see what raw tags were seen by Facebook when checking your page in our case they retrieved our Open Graph tags. *\[Figure-6\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/social-links/fb-share/cw-fbshare-figure6.png">![Figure-6](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/social-links/fb-share/cw-fbshare-figure6.png "Figure-6"){.uk-thumbnail .uk-thumbnail-mini}</a>

Next Facebook takes the raw tags and constructs a series of definitive Open Graph tags for the page. If the Open Graph tags in the head of the page were displayed correctly they should coincide with this section. *\[Figure-7\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/social-links/fb-share/cw-fbshare-figure7.png">![Figure-7](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/social-links/fb-share/cw-fbshare-figure7.png "Figure-7"){.uk-thumbnail .uk-thumbnail-mini}</a>

Next is a great way to actually see what will be shared when a button is clicked on that page. *\[Figure-8\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/social-links/fb-share/cw-fbshare-figure8.png">![Figure-8](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/social-links/fb-share/cw-fbshare-figure8.png "Figure-8"){.uk-thumbnail .uk-thumbnail-mini}</a>

**How do I update what Facebook has stored?**

1. If your site doesn't have any errors and Facebook can see and retrieved your page information you can wait up to 24 hours for your pages to automatically catch up.

2. You can also force a page to catch up using the **Fetch new scrape information** button at the top which will instructed Facebook to recheck the page now. If you see all the information is being displayed correctly when you scroll down to the  **When shared, this is what will be included** then the share button on that page should now share the correct information.

**Tip:** If you find the majority of your pages are displaying correctly but a particular page is being stubborn open up the **Debug Tool** and try the **Fetch new scrape information** button from the top to force it to catch up. If after fetching your page information everything is displaying correctly head back to your site and test your button again. 

## <a name="tips"></a>Quick Tips

1. If the image referenced by the Open Graph tags is too small Facebook will move onto another image that it finds on the page that meets the minimum size restrictions. FB will only use images that are at least 200x200 px and prefers images that are measured in multiples of 100 and are in a square format.

2. Facebook stores page information for up to 24 hours so any changes you make or if you have just brought your site online can take up to 24 hours to catch up.

3. Joomla 3.+ sites using Gzip compression will need to use the Gzip Help option in the System CW Gears plugin.

4. To use the Debugger Tool you will need to have a Facebook account and be logged in.

5. Stubborn pages, if you find the majority of your pages are displaying correctly but a particular page isn't drop by the Debug tool and try the **Fetch new scrape information** to force it to catch up. If everything is displaying correctly head back to your site and test your button again. 

## <a name="more-help"></a>Need More Help

<div class="uk-alert">Do you have a question that wasn't covered by this GUIDE? Try the <a href="https://coalaweb.com/support/documentation/category/social-links" target="_self">FAQ</a></div>

<div class="uk-alert">Do you have a question that wasn't covered by this GUIDE or the FAQ? Then it's time to drop by the <a href="https://coalaweb.com/forum/index" target="_self">Forum</a></div>