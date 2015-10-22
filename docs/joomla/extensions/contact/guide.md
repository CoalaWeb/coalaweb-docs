## Table of Contents
1.  [Overview](#overview)
2.  [Component Guide](#component-guide)
    -   [Control Panel](#control-panel)
    -   [Inbuilt Help](#help)
    -   [Extension Options](#options)
        - [1. General Contact Options](#options-general)
        - [2. Custom Fields](#options-custom)
        - [3. Messages and Warnings](#options-messages)
        - [4. Labels](#options-labels)
        - [5. Captcha](#options-captcha)
        - [6. Map](#options-map)
        - [7. Advanced](#options-advanced)
        - [8. Updates](#options-updates)
        - [9. Component Permissions](#options-permissions)
3.  [Contact \[M\]](#module)
    -   [General Display Options](#mod-general)
    -   [Custom Fields](#mod-custom)
    -   [Captcha](#mod-captcha)
    -   [Map](#mod-map)
    -   [Advanced](#mod-advanced)
    -   [Release Information](#mod-release)
4.  [Contact Tab \[Pro\]\[M\]](#tab)
    -   [General Display Options](#tab-general)
    -   [Layout and Style](#tab-style)
    -   [Custom Fields](#tab-custom)
    -   [Captcha](#tab-captcha)
    -   [Advanced](#tab-advanced)
    -   [Release Information](#tab-release)
5.  [Plugins](#plg)
    -   [Content Plugin - Contact \[Pro\]](#plg-content)
    -   [System Plugin - Mail Check](#plg-check)
    -   [Editor XTD Plugin - Contact \[Pro\]](#plg-xtd)
6.  [Need More Help?](#more-help)

## <a class="doc-top"  name="overview"></a>Overview

**CoalaWeb Contact** is a contact form extension packed full of options and designed to give website administrators a quick and easy way to place contact forms anywhere within their Joomla website.

<div class="uk-alert">When installing all the parts of the system will be installed at the same time making installing, upgrading and uninstalling a breeze.</div>

## <a name="component-guide"></a>Component

### <a name="control-panel"></a>Control Panel

The **Control Panel** as seen below is designed to be an easy starting point, think of it as the head quarters for the extension. While carrying out tasks you can easily jump from the **Control Panel** to the different sections and then return before moving onto the next one. *\[Figure-1\]*

![Figure-1](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/system-parts/com-contact.png "Figure-1"){.coalaweb-docs}

### <a name="help"></a>Inbuilt Help

In the control panel or the tool menu you have a help icon that when clicked will open a pop up wrapper of this specific guide. This gives you an easy way of checking the functionality of a particular item with out leaving the control panel. *\[Figure-2\]*

![Figure-2](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-help.png "Figure-2"){.coalaweb-docs}

### <a name="options"></a>Extension Options

In the control panel or the tool menu you have an options icon that when clicked will open a new window containing the various extension options.

### <a name="options-general"></a>1. General Options

<div class="uk-alert">The options below will influence the Content Plugin and both Contact Modules unless overridden in the module configuration.</div>

<div class="uk-alert">To make it easier to follow I have broken up the General settings into three parts.</div>

#### Part 1

The first thing you will need to do is decide if you want the forms to be sent to one address or for **Pro** subscribers give the user the option to select from a list of options.

<div class="uk-alert">You will need to setup at least one **Recipient Email** or the system will display an error message.</div>

If you have select **Single** then all you have to do is enter the email address that you want your forms to be sent to. *\[Figure-3a\]*

![Figure-3a](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-config-general1.png "Figure-3a"){.coalaweb-docs}

If you are using the **Pro** version and you have selected **Departments** then a new field will appear allowing you to enter each one separated by a comma in the following format. *\[Figure-3b\]*

        Dep 1:dep1@example.com,Dep 2:dep2@example.com

![Figure-3b](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-config-general1a.png "Figure-3b"){.coalaweb-docs}

Pro subscribers will also have two additional fields a CC Email and a BCC email. Next you have a **Default Subject** option this will display in the email subject followed by the submitters subject if you have chosen to display this option. 

Next is the **Mail From** option where you can choose to have the email sent by the **Contact Form User** or by the **Joomla Mail Settings**. In some cases you have will have to use the **Joomla Mail Settings** for the system to work correctly due to hosting or service provider restrictions.

Next you have an option to chose the format you wish the emails to be sent in. If you are using the **Core** version you will only have the **No HTML** option but for **Pro** users you will have two additional options of **Basic HTML** and **Rich HTML**. The next options allows you to define the ID of your templates **System Message** location but in the majority of cases the default will work fine. The last option in Part1 is **Redirection** after the mail has been successfully sent. 

The **Core** version gives you two options the first one is to return to the **Same Page** that the form was submitted on while the second one will return the user to the **Home Page** of your website. The **Pro** version has an additional **Custom URL** option that if chosen will redirect the user to the URL entered in the following **Custom URL** field. *\[Figure-3\]*

![Figure-3](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-config-general1b.png "Figure-3"){.coalaweb-docs}

#### Part 2

Next we have some **Field Display** options that will affect what and how items are displayed within the contact form. Firstly you have the option to turn on or off the display of the following fields **Email**, **Name**, **Subject** and **Message** and also if they are required. If you are using the **Pro** version you will also have two more options **Date From** and **Date To** these will display with a **Calendar** selector next to these fields. If you have chosen to display either of date input fields you can also chose the date format to be used. 

The available options coincide with Joomla's standard types such as **LC3**. The **Display Format** option will display an example of the currently acceptable format under the date fields which is handy when JavaScript is turned off on the users computer so they can still input the date manually using the correct format. 

The next option gives **Pro** users the ability to display a **Terms of Service** input field that can also be set to required. If you want to display the **TOS**  you will also need to enter an article **ID** in the **TOS Article ID** this is the article that will be displayed in a popup window so users can read before agreeing. Next you can chose to display a **Copy Me** field allowing users to receive a copy of the form when they submit it. 

The last two options are for the **Pro** subscribers and they allow you to set and display the **Character Limit** for the message field of the form. If displayed the **Character Limit** will count down as text is entered into the message field. *\[Figure-4\]*

![Figure-4](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-config-general2.png "Figure-4"){.coalaweb-docs}

#### Part 3

Lastly we have some **Layout & Style** options that will affect the look and feel of the contact form. The first one gives you the option to include the CSS included with the CoalaWeb Contact extension or not. The next option allows you to choose a **Theme** for the contact form. **Core** users only have two options while the **Pro** subscribers get three.

#### Creating your own theme

Creating a theme is easy, just copy the light folder found in:

    media → coalawebcontact → components → contact → themes

Give the theme a different name and edit the files as needed. All the folders located in the themes directory will automatically be listed in the **Form Theme** select list. 

Next you can choose the width of the contact form in %. The next option allows you to choose a **Button Style** for the contact form. **Core** users have the default or custom options while the **Pro** subscribers get 12 color options as well. The last two options allow you to choose the text to be displayed on the **Submit** button. *\[Figure-5\]*

![Figure-5](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-config-general3.png "Figure-5"){.coalaweb-docs}

### <a name="options-custom"></a>2. Custom Fields

In this section you can setup one custom field for **Core** users or up to three for **Pro** users. For each field you have several options the first one is if you want to display it at all. The next option is the type of custom field you want to use and you have the follow options **Text**, **Text Area** and **Select List**. If you have chosen to use a **Select List** then a new field will appear allowing you to enter each one separated by a comma in the following format. *\[Figure-5b\]*

        Option 1,Option 2,Option 3

![Figure-5b](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-config-custom1.png "Figure-5b"){.coalaweb-docs}

The next option is what text you want to be used for the form field **Label**. Next you can chose the **Hint** that will be displayed in the form field when empty. The last option is the message that will be displayed if you have set the custom field to **Required** and the user doesn't fill it in. *\[Figure-5c\]*

![Figure-5b](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-config-custom1a.png "Figure-5c"){.coalaweb-docs}

### <a name="options-messages"></a>3. Messages and Warnings

The next tab allows you to customize the **Messages and Warnings** displayed by the CoalaWeb Contact extension. Note: If your site is multilingual leave blank and use the language files. *\[Figure-6\]*

![Figure-6](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-config-messages.png "Figure-6"){.coalaweb-docs}

### <a name="options-labels"></a>4. Labels

The next tab allows you to customize the **Labels** displayed by the CoalaWeb Contact extension both in the forms and the sent e-mail. Note: If your site is multilingual leave blank and use the language files. *\[Figure-7\]*

![Figure-7](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-config-labels.png "Figure-7"){.coalaweb-docs}

### <a name="options-captcha"></a>5. Captcha

The next tab allows you to display a **Captcha** to attempt to reduce pesky spam. Lets start with the options that apply to both the **Core** and **Pro** versions of the extension. Firstly you have the option to pick what type of Captcha you wish to display. The **Core** users only get one option the basic question and answer type Captcha while **Pro** users get three. Next you get to choose if you want to display a title/hint above the Captcha.

#### Basic Captcha

The next two options are applicable when using the basic question and answer type Captcha \[The Default Captcha\]. They allow you to chose a question to be displayed and the answer to be check against before allowing the form to be submitted. The default question is:

    Question = How many wheels does a bicycle have?

    Answer = 2

Feel free to choose a question and answer but try to aim for a good balance between difficult to answer for a spam bot while not too annoying for a real user. Note: If your site is multilingual leave blank and use the language files. *\[Figure-8\]*

![Figure-8](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-config-captcha1.png "Figure-8"){.coalaweb-docs}

For the Pro subscribers you get two additional Captcha options.

#### Image Captcha

To allow the **Image Captcha** to function correctly your system must have both the **GD** and **FreeType** libraries installed and allow access to the **captcha_images.php** file located at:

    administrator/components/com_coalawebcontact/assets/captcha/captcha_images.php

Access is particularly important if you are using a **.htaccess** file for example to have the image captcha work with correctly while using **Admin Tools** you would open up the **htaccess Maker** and scroll down to the **Exceptions -> Allow direct access to these files** field and enter in line above. Once you have selected **Save and create .htaccess** your image captcha should display and function correctly. *\[Figure 9a\]*

![Figure-9a](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-config-captcha3.png "Figure-9a"){.coalaweb-docs}

#### ReCaptcha

CoalaWeb Contact integrates the inbuilt Joomla **Captcha - reCAPTCHA** plugin so if you haven't already set it up using the **Version 2** option read on.

To get started grab your **Site** and **Secret** keys by signing in with your Google account (create an account if you don't have one) here: [Create a reCAPTCHA key](https://www.google.com/recaptcha/admin/create). Once you have an account register your website domain, and Google will provide you with your ReCAPTCHA keys. 

Next head over to your plugin manager and filter by type **Captcha** and you should see the **Captcha - ReCaptcha** plugin listed. Once you have selected it from the list choose **2.0** for the **Version** and then enter the **Site key** and **Secret key** your received in the previous step. The last option is to display the captcha in a dark or light style once you selected save the plugin making sure it's published. Now you can feel free to select reCAPTCHA from the list of options in the CoalaWeb Contact extension. *\[Figure-9b\]*

<div class="uk-alert">TIP: If you are using the reCAPTCHA option with a contact form and you are short on space try the <em>reCAPTCHA Compact</em> option found in the <em>System - CW Gears</em> plugin.</div>

![Figure-9b](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-config-captcha2.png "Figure-9b"){.coalaweb-docs}

### <a name="options-map"></a>6. Map

If you are a **Pro** subscriber you also get the option to included a Google map with your contact form. The first option allows to globally turn on or off the display of a map and the second its location either at the **Top** or **Bottom** of the contact form. *\[Figure-22a\]*

![Figure-22a](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-config-map1.png "Figure-22a"){.coalaweb-docs}

<div class="uk-alert">To make it easier to explain I have broken up the rest of the map options into two parts.</div>

#### Part 1 - General Options

The first two options in this section are **Latitude** and **Longitude** there are several ways to get this info but I find the easiest one is by using this [website](http://mondeca.com/index.php/en/any-place-en). Next you can choose the **Default Zoom** this will depend on your particular situation. The last option in this section is the **Height** of the map and keep in mind that the width will be responsive based on the forms current container size. *\[Figure-22b\]*

![Figure-22b](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-config-map2.png "Figure-22b"){.coalaweb-docs}

#### Part 2 - Popup Options

To pin point a location on the map a pin with an accompanying popup message is provided. Give the popup a **Title** and some **Text** that will be display when the location pin is clicked and you can also set the max width if space is limited. *\[Figure-22c\]*

![Figure-22c](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-config-map3.png "Figure-22c"){.coalaweb-docs}

### <a name="options-advanced"></a>7. Advanced

In this section there is three options for **Pro** subscribers and two for **Core** users. Option one is to turn on or off the **Email Cloak** let me explain when to use this option. If you have disabled the native Joomla email cloak plugin or you are using a third party extension to cloak your emails please set the option below to No. *\[Figure-23\]*

The next option is only for **Pro** subscribers and it turns on or off the display of an editor button to make it easier to include the CoalaWeb Contact plugin code in your articles. *\[Figure-23\]*

The last button allows you to turn on or off the display of the **CoalaWeb Mail Check** button in your **Global Configuration** setting to help test and fault find your mail settings.

![Figure-23](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-config-advanced1.png "Figure-23"){.coalaweb-docs}

### <a name="options-updates"></a>8. Update Options

The CoalaWeb Contact extension integrates with the inbuilt **Joomla Update** system so both **Core** and **Pro** users can keep their extension up to date. For **Core** users when you see updates listed in the Joomla update manager so when you do see one feel free to select it and update from with in Joomla. For **Pro** subscribers you will be notified through the inbuilt Joomla update system but you will have to drop by **coalaweb.com** and download a copy of the latest release, this is to ensure that a user has a valid subscription.

<div class="uk-alert">The <em>Download ID</em> system is currently being reviewed.</div>

### <a name="options-permissions"></a>9.Component Permissions

The last tab contains the permission settings for the CoalaWeb Contact component. *\[Figure-12\]*

![Figure-12](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-config-permissions.png "Figure-12"){.coalaweb-docs}

# <a name="module"></a>Contact Module

![Module-Demo](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/system-parts/mod-contact.png "Contact Module-Demo"){.coalaweb-docs}

### <a name="mod-general"></a>General Display Options

<div class="uk-alert">The settings below will override any you have already set in the <em>Component Options</em>.</div>

<div class="uk-alert">To make it easier to follow I have broken up the General settings into four parts.</div>

#### Part 1

The first thing you will need to do is decide if you want the forms to be sent to one address or for **Pro** subscribers give the user the option to select from a list of options.

<div class="uk-alert">You will need to setup at least one <em>Recipient Email</em> or the system will display an error message.</div>

If you have select **Single** then all you have to do is enter the email address that you want your forms to be sent to. *\[Figure-13a\]*

![Figure-13a](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-mod-config-general1.png "Figure-13a"){.coalaweb-docs}

If you are using the **Pro** version and you have selected **Departments** then a new field will appear allowing you to enter each one separated by a comma in the following format. *\[Figure-3b\]*

        Dep 1:dep1@example.com,Dep 2:dep2@example.com

![Figure-13b](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-mod-config-general1a.png "Figure-13b"){.coalaweb-docs}

Pro subscribers will also have two additional fields a CC Email and a BCC email. Next you have a **Default Subject** option this will display in the email subject followed by the submitters subject if you have chosen to display this option. *\[Figure-13c\]*

![Figure-13c](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-mod-config-general1b.png "Figure-13c"){.coalaweb-docs}

#### Part 2

Next we have some **Field Display** options that will affect what and how items are displayed within the contact form. Firstly you have the option to turn on or off the display of the following fields **Email**, **Name**, **Subject** and **Message** and also if they are required. If you are using the **Pro** version you will also have two more options **Date From** and **Date To** these will display with a **Calendar** selector next to these fields. If you have chosen to display either of date input fields you can also chose the date format to be used. 

The available options coincide with Joomla's standard types such as **LC3**. The **Display Format** option will display an example of the currently acceptable format under the date fields which is handy when JavaScript is turned off on the users computer so they can still input the date manually using the correct format. 

The next option gives **Pro** users the ability to display a **Terms of Service** input field that can also be set to required. If you want to display the **TOS**  you will also need to enter an article **ID** in the **TOS Article ID** this is the article that will be displayed in a popup window so users can read before agreeing. Next you can chose to display a **Copy Me** field allowing users to receive a copy of the form when they submit it. 

The last two options are for the **Pro** subscribers and they allow you to set and display the **Character Limit** for the message field of the form. If displayed the **Character Limit** will count down as text is entered into the message field. *\[Figure-14a\]*

![Figure-14a](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-mod-config-general2.png "Figure-14a"){.coalaweb-docs}

#### Part 3

The next section covers **Redirection** after the mail has been successfully sent. The **Core** version gives you two options the first one is to return to the **Same Page** that the form was submitted on while the second one will return the user to the **Home Page** of your website. The **Pro** version has an additional **Custom URL** option that if chosen will redirect the user to the URL entered in the following **Custom URL** field. *\[Figure-14b\]*

![Figure-14b](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-mod-config-general2b.png "Figure-14b"){.coalaweb-docs}

#### Part 4

Lastly we have some **Layout & Style** options that will affect the look and feel of the contact form. The first option allows you to choose a **Theme** for the contact form. **Core** users only have two options while the **Pro** subscribers get three.

#### Creating your own theme

Creating a theme is easy, just copy the light folder found in:

    media → coalawebcontact → components → contact → themes

Give the theme a different name and edit the files as needed. All the folders located in the themes directory will automatically be listed in the **Form Theme** select list. 

Next you can choose the width of the contact form in %. The next option allows you to choose a **Button Style** for the contact form. **Core** users have the default or custom options while the **Pro** subscribers get 12 color options as well. The last two options allow you to choose the text to be displayed on the **Submit** button. *\[Figure-14b\]*

![Figure-14b](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-mod-config-general3.png "Figure-14b"){.coalaweb-docs}

### <a name="mod-custom"></a>Custom Fields

In this section you can choose to display one custom field for **Core** users or up to three for **Pro** users. The specifics for each of the custom fields can be found in the **component** configuration options. *\[Figure-15\]*

![Figure-15](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-mod-config-custom1.png "Figure-15"){.coalaweb-docs}

### <a name="mod-captcha"></a>Captcha

The next options group allows you to display a **Captcha** to attempt to reduce pesky spam. Lets start with the options that apply to both the
**Core** and **Pro** versions of the extension. Firstly you have the option to pick what type of captcha you wish to display the **Core** users only get one option the basic question and answer type Captcha while **Pro** users get three. Next you get to chose if you want to display a title/hint above the Captcha.

#### Basic Captcha

The next two options are applicable when using the basic question and answer Captcha they allow you to chose a question to be displayed and the answer to be check against before allowing the form to be submitted. The default question is:

    Question = How many wheels does a bicycle have?

    Answer = 2

Feel free to chose a question and answer but try to aim for a good balance between difficult to answer for a spam bot while not too annoying for a real user. Note: If your site is multilingual leave blank and use the language files. *\[Figure-16\]*

![Figure-16](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-mod-config-captcha1.png "Figure-16"){.coalaweb-docs}

<div class="alert">For the <em>Pro</em> subscribers you get two additional Captcha options.</div>

#### Image Captcha

To allow the **Image Captcha** to function correctly your system must have both the **GD** and **FreeType** libraries installed and allow access to the **captcha_images.php** file located at:

    administrator/components/com_coalawebcontact/assets/captcha/captcha_images.php

Access is particularly important if you are using a **.htaccess** file for example to have the image captcha work with correctly while using **Admin Tools** you would open up the **htaccess Maker** and scroll down to the **Exceptions -> Allow direct access to these files** field and enter in line above. Once you have selected **Save and create .htaccess** your image captcha should display and function correctly. *\[Figure 9a\]*

![Figure-9a](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-config-captcha3.png "Figure-9a"){.coalaweb-docs}

#### ReCaptcha

CoalaWeb Contact integrates the inbuilt Joomla **Captcha - reCAPTCHA** plugin so if you haven't already set it up using the **Version 2** option read on.

To get started grab your **Site** and **Secret** keys by signing in with your Google account (create an account if you don't have one) here: [Create a reCAPTCHA key](https://www.google.com/recaptcha/admin/create). Once you have an account register your website domain, and Google will provide you with your ReCAPTCHA keys. 

Next head over to your plugin manager and filter by type **Captcha** and you should see the **Captcha - ReCaptcha** plugin listed. Once you have selected it from the list choose **2.0** for the **Version** and then enter the **Site key** and **Secret key** your received in the previous step. The last option is to display the captcha in a dark or light style once you selected save the plugin making sure it's published. Now you can feel free to select reCAPTCHA from the list of options in the CoalaWeb Contact extension. *\[Figure-9b\]*

<div class="uk-alert">TIP: If you are using the reCAPTCHA option with a contact form and you are short on space try the <em>reCAPTCHA Compact</em> option found in the <em>System - CW Gears</em> plugin.</div>

![Figure-9b](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-config-captcha2.png "Figure-9b"){.coalaweb-docs}

### <a name="mod-map"></a>Map

If you are a **Pro** subscriber you also get the option to included a Google map with your contact form. The first option allows to globally turn on or off the display of a map and the second its location either at the **Top** or **Bottom** of the contact form. The last option in this section is the **Height** of the map and keep in mind that the width will be responsive based on the forms current container size. *\[Figure-24\]*

![Figure-24](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-mod-config-map.png "Figure-24"){.coalaweb-docs}


### <a name="mod-advanced"></a>Advanced Options

The CoalaWeb Contact module also has a few of what I consider **Advanced Options** such a **Module Class Suffix** and whether to use **Cache**including the **Cache Time**.  *\[Figure-18\]*

![Figure-18](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-mod-config-advanced.png "Figure-18"){.coalaweb-docs}

### <a name="mod-release"></a>Release Information

In this section you can find out information about the currently installed extension such as **Type**, **Version** and **Release Date**. *\[Figure-19\]*

![Figure-19](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-mod-config-r-info.png "Figure-19"){.coalaweb-docs}

# <a name="tab"></a>Contact Tab Module \[Pro\]

![Module-Demo](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/system-parts/mod-tab.png "Contact Tab Module Demo"){.coalaweb-docs}

### <a name="tab-general"></a>General Display Options

<div class="uk-alert">The settings below will override any you have already set in the <em>Component Options</em>.</div>

<div class="uk-alert">To make it easier to follow I have broken up the General settings into three parts.</div>

#### Part 1

The first thing you will need to do is decide if you want the forms to be sent to one address or for **Pro** subscribers give the user the option to select from a list of options.

<div class="uk-alert">You will need to setup at least one <em>Recipient Email</em> or the system will display an error message.</div>

If you have select **Single** then all you have to do is enter the email address that you want your forms to be sent to. *\[Figure-13a\]*

![Figure-13a](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-mod-config-general1.png "Figure-13a"){.coalaweb-docs}

If you are using the **Pro** version and you have selected **Departments** then a new field will appear allowing you to enter each one separated by a comma in the following format. *\[Figure-3b\]*

        Dep 1:dep1@example.com,Dep 2:dep2@example.com

![Figure-13b](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-mod-config-general1a.png "Figure-13b"){.coalaweb-docs}

Pro subscribers will also have two additional fields a CC Email and a BCC email. Next you have a **Default Subject** option this will display in the email subject followed by the submitters subject if you have chosen to display this option. *\[Figure-13c\]*

![Figure-13c](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-mod-config-general1b.png "Figure-13c"){.coalaweb-docs}

#### Part 2

Next we have some **Field Display** options that will affect what and how items are displayed within the contact form. Firstly you have the option to turn on or off the display of the following fields **Email**, **Subject** and **Message** and also if they are required.

The last two options are for the **Pro** subscribers and they allow you to set and display the **Character Limit** for the message field of the form. If displayed the **Character Limit** will count down as text is entered into the message field. *\[Figure-25a\]*

![Figure-25a](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-tab-config-general1.png "Figure-25a"){.coalaweb-docs}

#### Part 3

The next section covers **Redirection** after the mail has been successfully sent. The **Core** version gives you two options the first one is to return to the **Same Page** that the form was submitted on while the second one will return the user to the **Home Page** of your website. The **Pro** version has an additional **Custom URL** option that if chosen will redirect the user to the URL entered in the following **Custom URL** field. *\[Figure-14b\]*

![Figure-14b](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-mod-config-general2b.png "Figure-14b"){.coalaweb-docs}

### <a name="tab-style"></a>Layout and Style

<div class="uk-alert">The settings below will override any you have already set in the <em>Component Options</em>.</div>

<div class="uk-alert">To make it easier to follow I have broken up the General settings into three parts.</div>

#### Part 1

The first few options in this section control the layout of the Tab module. You can choose to display the module at the top or bottom on either side and you can also set the offset in pixels. *\[Figure-25b\]*

![Figure-25b](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-tab-config-style1.png "Figure-25b"){.coalaweb-docs}

#### Part 2

Next you can chose how you want the module to behave on mobile devices. You can turn on or off it's display on **Tablets** and or **Mobiles**. You can also set the trigger widths for both **Tablets** and **Mobiles** in pixels.

The next option allows you to choose a **Theme** for the contact form. **Core** users only have two options while the **Pro** subscribers get three.

#### Creating your own theme

Creating a theme is easy, just copy the light folder found in:

    media → coalawebcontact → components → contact → themes

Give the theme a different name and edit the files as needed. All the folders located in the themes directory will automatically be listed in the **Form Theme** select list. 

The next option allows you to choose a **Button Style** for the contact form. **Core** users have the default or custom options while the **Pro** subscribers get 12 color options as well. The last two options allow you to choose the text to be displayed on the **Submit** button. *\[Figure-25c\]*

![Figure-25c](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-tab-config-style2.png "Figure-25c"){.coalaweb-docs}

#### Part 3

The last few options are related to the styling of the **Tab**. First you can choose from several icon options that will be displayed on the tab. The last two options allow you to choose the complete slide out Tabs's background and hover colors using a color selector. *\[Figure-25d\]*

![Figure-25d](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-tab-config-style3.png "Figure-25d"){.coalaweb-docs}

### <a name="tab-custom"></a>Custom Fields

In this section you can choose to display one custom field for **Core** users or up to three for **Pro** users. The specifics for each of the custom fields can be found in the **component** configuration options. *\[Figure-15\]*

![Figure-15](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-mod-config-custom1.png "Figure-15"){.coalaweb-docs}

### <a name="tab-captcha"></a>Captcha

The next options group allows you to display a **Captcha** to attempt to reduce pesky spam. Lets start with the options that apply to both the
**Core** and **Pro** versions of the extension. Firstly you have the option to pick what type of captcha you wish to display the **Core** users only get one option the basic question and answer type Captcha while **Pro** users get three. Next you get to chose if you want to display a title/hint above the Captcha.

#### Basic Captcha

The next two options are applicable when using the basic question and answer Captcha they allow you to chose a question to be displayed and the answer to be check against before allowing the form to be submitted. The default question is:

    Question = How many wheels does a bicycle have?

    Answer = 2

Feel free to chose a question and answer but try to aim for a good balance between difficult to answer for a spam bot while not too annoying for a real user. Note: If your site is multilingual leave blank and use the language files. *\[Figure-16\]*

![Figure-16](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-mod-config-captcha1.png "Figure-16"){.coalaweb-docs}

<div class="alert">For the <em>Pro</em> subscribers you get two additional Captcha options.</div>

#### Image Captcha

To allow the **Image Captcha** to function correctly your system must have both the **GD** and **FreeType** libraries installed and allow access to the **captcha_images.php** file located at:

    administrator/components/com_coalawebcontact/assets/captcha/captcha_images.php

Access is particularly important if you are using a **.htaccess** file for example to have the image captcha work with correctly while using **Admin Tools** you would open up the **htaccess Maker** and scroll down to the **Exceptions -> Allow direct access to these files** field and enter in line above. Once you have selected **Save and create .htaccess** your image captcha should display and function correctly. *\[Figure 9a\]*

![Figure-9a](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-config-captcha3.png "Figure-9a"){.coalaweb-docs}

#### ReCaptcha

CoalaWeb Contact integrates the inbuilt Joomla **Captcha - reCAPTCHA** plugin so if you haven't already set it up using the **Version 2** option read on.

To get started grab your **Site** and **Secret** keys by signing in with your Google account (create an account if you don't have one) here: [Create a reCAPTCHA key](https://www.google.com/recaptcha/admin/create). Once you have an account register your website domain, and Google will provide you with your ReCAPTCHA keys. 

Next head over to your plugin manager and filter by type **Captcha** and you should see the **Captcha - ReCaptcha** plugin listed. Once you have selected it from the list choose **2.0** for the **Version** and then enter the **Site key** and **Secret key** your received in the previous step. The last option is to display the captcha in a dark or light style once you selected save the plugin making sure it's published. Now you can feel free to select reCAPTCHA from the list of options in the CoalaWeb Contact extension. *\[Figure-9b\]*

<div class="uk-alert">TIP: If you are using the reCAPTCHA option with a contact form and you are short on space try the <em>reCAPTCHA Compact</em> option found in the <em>System - CW Gears</em> plugin.</div>

![Figure-9b](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-config-captcha2.png "Figure-9b"){.coalaweb-docs}

### <a name="tab-advanced"></a>Advanced Options

The CoalaWeb Contact Tab module also has a few of what I consider **Advanced Options** such a **Module Class Suffix** and whether to use **Cache**including the **Cache Time**.  *\[Figure-18\]*

![Figure-18](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-mod-config-advanced.png "Figure-18"){.coalaweb-docs}

### <a name="tab-release"></a>Release Information

In this section you can find out information about the currently installed extension such as **Type**, **Version** and **Release Date**. *\[Figure-19\]*

![Figure-19](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-mod-config-r-info.png "Figure-19"){.coalaweb-docs}

## <a name="plg"></a>Plugins

### <a name="plg-content"></a>Content Plugin - Contact \[Pro\]

The CoalaWeb Contact plugin gives you even more flexibility by allowing you to place one or more contact forms anywhere within your content. All of the configuration options for this particular plugin can be found in the accompanying component under **Extension Options**. If you can't see the contact form displayed in your content make sure you have the plugin installed and published and that you have selected the appropriate configuration options.

The easiest way to use the plugin is in conjunction with the article editor button which when clicked will add the necessary code to your page in the following format.

        {coalaweb-contact-form id=123}

<div class="uk-alert">If you have multiple forms then make sure to give them a different <em>ID</em> to stop potential conflicts.</div>

![Content-PLG-Demo](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/system-parts/plg-contact.png "Content PLG Demo"){.coalaweb-docs}

### <a name="plg-check"></a>System Plugin - Mail Check

The CoalaWeb Mail Check plugin allows you to check your mail settings without having to save each time you make changes. All you need to do is make some changes to your **Mail** settings and then click the button to check if they function correctly. If there is an error just make the necessary changes and click the button again to test them, it's that easy!

<div class="uk-alert">You can disable this button from displaying from within the component options.</div>

![Mail Check](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/system-parts/plg-mailcheck.png "Mail Check Demo"){.coalaweb-docs}

### <a name="plg-xtd"></a>Editor XTD Plugin - Contact \[Pro\]

The **Editor XTD** plugin makes adding a contact form to your Joomla content a one click process. Just place the cursor where you want the form to be displayed and then click the **Insert Contact** button displayed at the bottom of the editor.

<div class="uk-alert">You can disable this button from displaying from within the component options.</div>

![XTD-PLG-Button](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/system-parts/plg-btncontact.png "XTD PLG Demo"){.coalaweb-docs}

### <a name="more-help"></a>Need more help?

<div class="uk-alert">Do you have a question that wasn't covered by this GUIDE? Try the <a href="http://coalaweb.com/support/documentation/category/contact" target="_self">FAQ</a></div>

<div class="uk-alert">Do you have a question that wasn't covered by this GUIDE or the FAQ? Then it's time to drop by the <a href="http://coalaweb.com/forum/index" target="_self">Forum</a></div>
