## Table of Contents

1.  [Intro](#intro)
2.  [Guide](#guide)
5.  [Things to note](#notes)
6.  [Need More Help?](#more-help)

## <a name="intro"></a>Intro

YooTheme templates don’t come with any specific K2 formating but it's easy to take advantage of some of the inbuilt features of Warp and get them working with your K2 content as well. In this guide we will be getting the fantastic pagination that comes built into Warp and applying it to k2. Don’t worry it’s an easy process just follow steps below.

## <a name="guide"></a>Guide

### Step 1

To get started log into your Joomla admin area then head over to the **Template Manager** and lastly open your YooTheme template for editing. In this example we will be using the **Nano 3** template but this should work fine for any modern YooTheme template. *\[Figure-1\]*

![Figure-1](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-tips/yt-k2-pagination/yt-k2-pagination-3.png "Figure-1"){.coalaweb-docs}

### Step 2

In the next window select the **Options** tab from the top then **Settings** from the left and finally click the **Customizer** button so we can get started creating our custom style. *\[Figure-2\]*

![Figure-2](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-tips/yt-k2-pagination/yt-k2-pagination-4.png "Figure-2"){.coalaweb-docs}

### Step 3

In the next window select your favorite style option from **Select a style** drop down list in the top left and then click **Copy**. In the pop up window give your new custom style a name and click **OK** then click **Save** from the bottom left to start the compiling process for your new style. *\[Figure-3\]*

![Figure-3](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-tips/yt-k2-pagination/yt-k2-pagination-5.png "Figure-3"){.coalaweb-docs}

### Step 4

Now before we start modifying our new style we have to make sure its being used this will let us see our hard work in action, To do this select **Layouts** from the left **Warp** menu then under **Style** select our newly created style and lastly click **Save and close** from the top Joomla menu. *\[Figure-4\]*

![Figure-4](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-tips/yt-k2-pagination/yt-k2-pagination-6.png "Figure-4"){.coalaweb-docs}

### Step 5

Now we need a file from warp and the easiest way to get it is by extracting your template and grabbing it from inside the warp directory. The file we are looking for is in this directory:

`yoo_template_name/warp/systems/joomla/layouts`

The file is called:

`pagination.php`

Once you find it make a copy to an appropriate location for editing. *\[Figure-5\]*

![Figure-5](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-tips/yt-k2-pagination/yt-k2-pagination-7.png "Figure-5"){.coalaweb-docs}

### Step 6

Now open up the file in your favorite text editor and look for this line:

`if (in_array(JFactory::getApplication()->scope, array('com_content', 'com_finder', 'com_search', 'com_tags'))) {`

Now that we have found it we want to append **com_k2** to the end of the array so it looks like this:

`if (in_array(JFactory::getApplication()->scope, array('com_content', 'com_finder', 'com_search', 'com_tags', 'com_k2'))) {`

**Note:** Make sure to use a comma and surround it with inverted commas.

Now save the file and we are ready to upload it to our website so the net step is to open up your FTP client and connect to your site. We are going to have to create a directory for our new layout inside the custom style we created earlier so open your template directory then move into:

`yoo_template_name/styles/your_custom_style`

Next create a **layouts** directory inside this location. *\[Figure-6\]*

![Figure-6](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-tips/yt-k2-pagination/yt-k2-pagination-8.png "Figure-5"){.coalaweb-docs}

### Step 7

Now you can upload your edited **pagination.php** file into the new **layouts** directory then clear your Joomla and Browser cache and lastly refresh your website to see your awesome new pagination in action. *\[Figure-7\]*

![Figure-7](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-tips/yt-k2-pagination/yt-k2-pagination-2.png "Figure-7"){.coalaweb-docs}

### All Done

Thats it! Now you have perfectly styled pagination that matches your template!

## <a name="notes"></a>Things to note

-   Joomla version: 3.4
-   K2 version: 2.6.9
-   YooTheme template: Nano 3 Joomla 3.3
-   YooTheme template version: 1.0.15

## <a name="more-help"></a>Need More Help

***

<div class="uk-alert">Do you have a question that wasn't covered by this GUIDE or the FAQ? Then it's time to drop by the <a href="https://coalaweb.com/forum/index" target="_self">Forum</a></div>