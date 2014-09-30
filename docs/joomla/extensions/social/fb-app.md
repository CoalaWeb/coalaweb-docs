## Table of Contents
1.  [Guide](#guide)
2.  [Need More Help?](#more-help)

## <a name="guide"></a>Guide to creating a Facebook Application
As you know, CoalaWeb Social Links allows you to share content through many social networks, including Facebook. Up until version 0.1.8 the Facebook share options of the **Social Links** and **Tabs** modules had been carried out using the Facebook **Sharer** code. But recently, Facebook announced that they have deprecated this code in preference of their new **Share Dialog** system, which requires a Facebook **App ID**.

To get a Facebook App ID requires you to first create a Facebook Application but don’t worry it’s an easy process which we will walk your through in the following guide.

### <a name="step-1"></a>Step 1
To get started lets head over to the Facebook developer's [website](https://developers.facebook.com) You will need to log into your Facebook account using your normal credentials before being able to access this page. *\[Figure-1\]*

![Figure-1](images/docs/joomla/extensions/social-links/fb/cw-fbapp-figure1.png "Figure-1"){.coalaweb-docs}

Now that we are in the **Developers** section of Facebook we can start creating out new App. First select the **Apps** dropdown menu from the top and choose **Add a New App**. *\[Figure-2\]*

![Figure-2](images/docs/joomla/extensions/social-links/fb/cw-fbapp-figure2.png "Figure-2"){.coalaweb-docs}

In the next window select **Website** from the options. *\[Figure-3\]*

![Figure-3](images/docs/joomla/extensions/social-links/fb/cw-fbapp-figure3.png "Figure-3"){.coalaweb-docs}

In the next window select **Skip Quickstart** from the top right. *\[Figure-4\]*

![Figure-4](images/docs/joomla/extensions/social-links/fb/cw-fbapp-figure4.png "Figure-4"){.coalaweb-docs}

In the **Create a New App** window give your new application a **Display Name**.

<span class="info" markdown="1">This will be seen in the bottom of the pop up **Share** dialog so something related to your website is best.</span>

You can leave the **Namespace** blank and **No** for the test version question. Lastly on this page you need to choose a **Category** for the App in this example I have chosen **Utilities** but for more info on categories try this [Link](https://developers.facebook.com/docs/games/appcenter/categories) *\[Figure-5\]* 

![Figure-5](images/docs/joomla/extensions/social-links/fb/cw-fbapp-figure5.png "Figure-5"){.coalaweb-docs}

When you click **Create App** you will be confronted with a Captcha so fill it in and click **Submit**. *\[Figure-6\]*

![Figure-6](images/docs/joomla/extensions/social-links/fb/cw-fbapp-figure6.png "Figure-6"){.coalaweb-docs}

###Congratulations! You’ve just created a Facebook App!

You should now be looking at your newly created application, you will note that under your **Application's Name** there is the sentence:

**This app is in development mode**

We still have a couple more steps before we are ready to use the **App ID**. *\[Figure-7\]*

![Figure-7](images/docs/joomla/extensions/social-links/fb/cw-fbapp-figure7.png "Figure-7"){.coalaweb-docs}

On the left side of your **Dashboard**, click **Settings** from the menu and make sure you looking at the **Basic** tab. In this window you will need to enter the **App Domains** and **Contact Email** for your app. *\[Figure-8\]*

<span class="tip" markdown="1">Do not include the **http** part of the domain.</span>

![Figure-8](images/docs/joomla/extensions/social-links/fb/cw-fbapp-figure8.png "Figure-8"){.coalaweb-docs}

Before clicking **Save Changes** we need to add a platform so yes you guessed it we will now use the **Add Platform** button. *\[Figure-9\]*

![Figure-9](images/docs/joomla/extensions/social-links/fb/cw-fbapp-figure9.png "Figure-9"){.coalaweb-docs}

From the next window choose **Website** for your platform. *\[Figure-10\]*

![Figure-10](images/docs/joomla/extensions/social-links/fb/cw-fbapp-figure10.png "Figure-10"){.coalaweb-docs}

In the next window enter your website address into the **Site URL** field and then choose **Save Changes**. *\[Figure-11\]*

<span class="tip" markdown="1">You **DO** want to include the full URL, including the http:// </span>

![Figure-11](images/docs/joomla/extensions/social-links/fb/cw-fbapp-figure11.png "Figure-11"){.coalaweb-docs}

Lets now make your App live and available to all users. To do this click the **Status & Review** option from menu to the left and then toggle the button at the top that says **Do you want to make this app and all its live features available to the general public?**. *\[Figure-12\]*

![Figure-12](images/docs/joomla/extensions/social-links/fb/cw-fbapp-figure12.png "Figure-12"){.coalaweb-docs}

Once you select **Yes** you will be confronted with a confirmation screen select **Confirm**. *\[Figure-13\]*

![Figure-13](images/docs/joomla/extensions/social-links/fb/cw-fbapp-figure13.png "Figure-13"){.coalaweb-docs}

Now when you are returned to the **Dashboard** you will see a solid green circle next to your **Applications Name** and under it the sentence:

**This app is public and available to all users**  *\[Figure-14\]*

![Figure-14](images/docs/joomla/extensions/social-links/fb/cw-fbapp-figure14.png "Figure-14"){.coalaweb-docs}

###Your new Application ID is ready for use in CoalaWeb Social Links!

## <a name="more-help"></a>Need More Help

<span class="tip" markdown="1">Do you have a question that wasn't covered by the GUIDE? Try the [FAQ](http://coalaweb.com/support-menu/documentation/item/coalaweb-social-links-faq).</span>

<span class="tip" markdown="1">Do you have a question that wasn't covered by the GUIDE or the FAQ? Then it's time to drop by the [Forum](http://coalaweb.com/forum/index) I'm sure we can help.</span>