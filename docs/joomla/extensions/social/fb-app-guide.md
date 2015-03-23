## Table of Contents
1.  [Register](#register)
2.  [Guide](#guide)
3.  [Need More Help?](#more-help)

## <a name="register"></a>Register as a Developer
You need to have your personal Facebook profile registered as a **Developer** before you can create and manage a **Facebook App**. If you already have a Facebook account and are registered as a developer jump down to the [Guide](#guide) if not read on.

First navigate to Facebook.com and login with your personal Facebook account. If you don't already have one you’ll need to create one now. 

Note: If you are only using Facebook to manage pages, these instructions will not work you will need a personal Facebook account to continue.

Next go to https://developers.facebook.com/apps and click on the green **Register as a Developer** button in the upper right. You will more than likely have to verify your Facebook account via phone. Once you have finished verifying your account click the **Register as a Developer** button and you will be confronted with a popup. *\[Figure-1\]*

![Figure-1](http://cdn.coalaweb.com/images/docs/joomla-extensions/social-links/fb/cw-fbapp-figure1.png "Figure-1"){.coalaweb-docs}

Check the **Accept Terms** box and click **Continue** in the next step you can either skip or complete all the information but keep in mind the answer aren'y super important. I recommend unchecking the box at the bottom to not receive emails but its up to you.

Click **Done** and you are now an official Facebook Developer!

## <a name="guide"></a>Guide to creating a Facebook Application
As you know, CoalaWeb Social Links allows you to share content through many social networks, including Facebook. Up until version 0.1.8 the Facebook share options of the **Social Links** and **Tabs** modules had been carried out using the Facebook **Sharer** code. But recently, Facebook announced that they have deprecated this code in preference of their new **Share Dialog** system, which requires a Facebook **App ID**.

To get a Facebook App ID requires you to first create a Facebook Application but don’t worry it’s an easy process which we will walk your through in the following guide.

### <a name="step-1"></a>Step 1
To get started lets head over to the Facebook developer's [website](https://developers.facebook.com) You will need to log into your Facebook account using your normal credentials before being able to access this page. *\[Figure-1a\]*

![Figure-1a](http://cdn.coalaweb.com/images/docs/joomla-extensions/social-links/fb/cw-fbapp-figure1a.png "Figure-1a"){.coalaweb-docs}

### <a name="step-2"></a>Step 2
Now that we are in the **Developers** section of Facebook we can start creating out new App. First select the **Apps** dropdown menu from the top and choose **Add a New App**. *\[Figure-2\]*

![Figure-2](http://cdn.coalaweb.com/images/docs/joomla-extensions/social-links/fb/cw-fbapp-figure2.png "Figure-2"){.coalaweb-docs}

### <a name="step-3"></a>Step 3
In the next window select **Website** from the options. *\[Figure-3\]*

![Figure-3](http://cdn.coalaweb.com/images/docs/joomla-extensions/social-links/fb/cw-fbapp-figure3.png "Figure-3"){.coalaweb-docs}

### <a name="step-4"></a>Step 4
In the next window select **Skip Quickstart** from the top right. *\[Figure-4\]*

![Figure-4](http://cdn.coalaweb.com/images/docs/joomla-extensions/social-links/fb/cw-fbapp-figure4.png "Figure-4"){.coalaweb-docs}

### <a name="step-5"></a>Step 5
In the **Create a New App** window give your new application a **Display Name**.

<div class="uk-alert">This will be seen in the bottom of the pop up <em>Share</em> dialog so something related to your website is best.</div>

You can leave the **Namespace** blank and **No** for the test version question. Lastly on this page you need to choose a **Category** for the App in this example I have chosen **Utilities** but for more info on categories try this [Link](https://developers.facebook.com/docs/games/appcenter/categories) *\[Figure-5\]* 

![Figure-5](http://cdn.coalaweb.com/images/docs/joomla-extensions/social-links/fb/cw-fbapp-figure5.png "Figure-5"){.coalaweb-docs}

### <a name="step-6"></a>Step 6
When you click **Create App** you will be confronted with a Captcha so fill it in and click **Submit**. *\[Figure-6\]*

![Figure-6](http://cdn.coalaweb.com/images/docs/joomla-extensions/social-links/fb/cw-fbapp-figure6.png "Figure-6"){.coalaweb-docs}

###Congratulations! You’ve just created a Facebook App!

### <a name="step-7"></a>Step 7
You should now be looking at your newly created application, you will note that under your **Application's Name** there is the sentence:

**This app is in development mode**

We still have a couple more steps before we are ready to use the **App ID**. *\[Figure-7\]*

![Figure-7](http://cdn.coalaweb.com/images/docs/joomla-extensions/social-links/fb/cw-fbapp-figure7.png "Figure-7"){.coalaweb-docs}

### <a name="step-8"></a>Step 8
On the left side of your **Dashboard**, click **Settings** from the menu and make sure you looking at the **Basic** tab. In this window you will need to enter the **App Domains** and **Contact Email** for your app. *\[Figure-8\]*

<div class="uk-alert">For the <em>App Domains</em> make sure to enter your website domain i.e where the extension is installed.</div>

<div class="uk-alert">Do not include the <em>http</em> part of the domain.</div>

![Figure-8](http://cdn.coalaweb.com/images/docs/joomla-extensions/social-links/fb/cw-fbapp-figure8.png "Figure-8"){.coalaweb-docs}

### <a name="step-9"></a>Step 9
Before clicking **Save Changes** we need to add a platform so yes you guessed it we will now use the **Add Platform** button. *\[Figure-9\]*

![Figure-9](http://cdn.coalaweb.com/images/docs/joomla-extensions/social-links/fb/cw-fbapp-figure9.png "Figure-9"){.coalaweb-docs}

### <a name="step-10"></a>Step 10
From the next window choose **Website** for your platform. *\[Figure-10\]*

![Figure-10](http://cdn.coalaweb.com/images/docs/joomla-extensions/social-links/fb/cw-fbapp-figure10.png "Figure-10"){.coalaweb-docs}

### <a name="step-11"></a>Step 11
In the next window enter your website address into the **Site URL** field and then choose **Save Changes**. *\[Figure-11\]*

<div class="uk-alert">You <em>DO</em> want to include the full URL, including the http:// </div>

![Figure-11](http://cdn.coalaweb.com/images/docs/joomla-extensions/social-links/fb/cw-fbapp-figure11.png "Figure-11"){.coalaweb-docs}

### <a name="step-12"></a>Step 12
Lets now make your App live and available to all users. To do this click the **Status & Review** option from menu to the left and then toggle the button at the top that says **Do you want to make this app and all its live features available to the general public?**. *\[Figure-12\]*

![Figure-12](http://cdn.coalaweb.com/images/docs/joomla-extensions/social-links/fb/cw-fbapp-figure12.png "Figure-12"){.coalaweb-docs}

### <a name="step-13"></a>Step 13
Once you select **Yes** you will be confronted with a confirmation screen select **Confirm**. *\[Figure-13\]*

![Figure-13](http://cdn.coalaweb.com/images/docs/joomla-extensions/social-links/fb/cw-fbapp-figure13.png "Figure-13"){.coalaweb-docs}

### <a name="step-14"></a>Step 14
Now when you are returned to the **Dashboard** you will see a solid green circle next to your **Applications Name** and under it the sentence:

**This app is public and available to all users**  *\[Figure-14\]*

![Figure-14](http://cdn.coalaweb.com/images/docs/joomla-extensions/social-links/fb/cw-fbapp-figure14.png "Figure-14"){.coalaweb-docs}

###Your new App ID is now ready for use!

## <a name="more-help"></a>Need More Help

<div class="uk-alert">Do you have a question that wasn't covered by this GUIDE? Try the <a href="http://coalaweb.com/support/documentation/category/social-links" target="_self">FAQ</a></div>

<div class="uk-alert">Do you have a question that wasn't covered by this GUIDE or the FAQ? Then it's time to drop by the <a href="http://coalaweb.com/forum/index" target="_self">Forum</a></div>