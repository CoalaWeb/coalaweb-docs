## Table of Contents
1.  [Component Guide](#component-guide)
    -   [Control Panel](#control-panel)
    -   [Inbuilt Help](#help)
    -   [Extension Options](#options)
        - [1. General Contact Options](#options-general)
        - [2. Custom Fields](#options-custom)
        - [3. Messages and Warnings](#options-messages)
        - [4. Labels](#options-labels)
        - [5. Captcha](#options-captcha)
        - [6. Advanced](#options-advanced)
        - [7. Where Is My Download ID \[Pro\]](#options-downloadid)
        - [8. Component Permissions](#options-permissions)
2.  [Contact Module Guide](#module)
    -   [General Display Options](#mod-general)
    -   [Custom Fields](#mod-general)
    -   [Captcha](#mod-captcha)
    -   [Advanced](#mod-advanced)
    -   [Release Information](#mod-release)
3.  [Plugin Guide \[Pro\]](#plg)
    -   [Content Plugin - Contact](#plg-content)
    -   [Editor XTD Plugin - Contact](#plg-xtd)
4.  [Need More Help?](#more-help)

## <a class="doc-top" name="component-guide"></a>Component
### <a name="control-panel"></a>Control Panel

The **Control Panel** as seen below is designed to be an easy starting point, think of it as the head quarters for the extension. While carrying out tasks you can easily jump from the **Control Panel** to the different sections and then return before moving onto the next one. *\[Figure-1\]*

![Figure-1](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-cpanel.png "Figure-1"){.coalaweb-docs}

### <a name="help"></a>Inbuilt Help

In the control panel or the tool menu you have a help icon that when clicked will open a pop up wrapper of this specific guide. This gives you an easy way of checking the functionality of a particular item with out leaving the control panel. *\[Figure-2\]*

![Figure-2](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-help.png "Figure-2"){.coalaweb-docs}

### <a name="options"></a>Extension Options

In the control panel or the tool menu you have an options icon that when clicked will open a new window containing the various extension options.

### <a name="options-general"></a>1. General Options

<div class="uk-alert">The options below will influence the Content Plugin [Pro] and the Contact Module unless overridden in the module configuration.</div>

<div class="uk-alert">To make it easier to follow I have broken up the General settings into three parts.</div>

#### Part 1

The first thing that will need to be filled in is the **Recipient Email** without this the system will display an error message. If you have purchased a Pro subscription you will also have two additional fields a CC Email and a BCC email. Next you have a **Default Subject** option this will display in the email subject followed by the submitters subject if you have chosen to display this option. 

Next is the **Mail From** option where you can choose to have the email sent by the **Contact Form User** or by the **Joomla Mail Settings**. In some cases you have will have to use the **Joomla Mail Settings** for the system to work correctly due to hosting or service provider restrictions.

Next you have an option to chose the format you wish the emails to be sent in. If you are using the core version you will only have the **No HTML** optionbut for Pro users you will have two additional options of **Basic HTML** and **Rich HTML**. The last option in Part1 is **Redirection** after the mail has been successfully sent. 

The **Core** version gives you two options the first one is to return to the **Same Page** that the form was submitted on while the second one will return the user to the **Home Page** of your website. The **Pro** version has an additional **Custom URL** option that if chosen will redirect the user to the URL entered in the following **Custom URL** field. *\[Figure-3\]*

![Figure-3](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-config-general1.png "Figure-3"){.coalaweb-docs}

#### Part 2

Next we have some **Field Display** options that will affect what and how items are displayed within the contact form. Firstly you have the option to turn on or off the display of the following fields **Name**, **Subject** and **Message** and also if they are required. If you are using the **Pro** version you will also have two more options **Date From** and **Date To** these will display with a **Calendar** selector next to these fields. If you have chosen to display either of date input fields you can also chose the date format to be used. 

The available options coincide with Joomla's standard types such as **LC3**. The **Display Format** option will display an example of the currently acceptable format under the date fields which is handy when JavaScript is turned off on the users computer so they can still input the date manually using the correct format. 

The next option gives **Pro** users the ability to display a **Terms of Service** input field that can also be set to required. If you want to display the **TOS**  you will also need to enter an article **ID** in the **TOS Article ID** this is the article that will be displayed in a popup window so users can read before agreeing. Next you can chose to display a **Copy Me** field allowing users to receive a copy of the form when they submit it. 

The last two options are for the **Pro** subscribers and they allow you to set and display the **Character Limit** for the message field of the form. If displayed the **Character Limit** will count down as text is entered into the message field. *\[Figure-4\]*

![Figure-4](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-config-general2.png "Figure-4"){.coalaweb-docs}

#### Part 3

Lastly we have some **Layout & Style** options that will affect the look
and feel of the contact form. The first one gives you the option to
include the CSS included with the CoalaWeb Contact extension or not. The
next option allows you to choose a **Theme** for the contact form.
**Core** users only have one option while the **Pro** subscribers get
two.

#### Creating your own theme

Creating a theme is easy, just copy the light folder found in:

    media → coalawebcontact → components → contact → themes

Give the theme a differnt name and edit the files as needed. All the
folders located in the themes directory will automatically be listed in
the **Form Theme** select list. Next you can choose the width of the
contact form in %. The next option allows you to choose a **Button
Style** for the contact form. **Core** users only have the default
option while the **Pro** subscribers get 6 color options as well. The
last two options allow you to choose the text to be displayed on the
**Submit** button at the bottom of the contact form and for the **Pro**
users the button displayed at the bottom of the editor window allowing
you to insert a form into your content. *\[Figure-5\]*

![Figure-5](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-config-general3.png "Figure-5"){.coalaweb-docs}

### <a name="options-custom"></a>2. Custom Fields

In this section you can setup one custom field for **Core** users or up to three for **Pro** users. For each filed you have several options the first one is if you want to display it at all. The next option is what text you want used as the form field **Label**. Next you can chose the **Hint** that will be displayed in the form field when empty. The last option is the message that will be displayed if you have set the custom field to **Required** and the user doesn't fill it in. *\[Figure-5b\]*

![Figure-5b](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-config-custom1.png "Figure-5b"){.coalaweb-docs}

### <a name="options-messages"></a>3. Messages and Warnings

The next tab allows you to customize the **Messages and Warnings**
displayed by the CoalaWeb Contact extension. Note: If your site is
multilingual leave blank and use the language files. *\[Figure-6\]*

![Figure-6](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-config-messages.png "Figure-6"){.coalaweb-docs}

### <a name="options-labels"></a>4. Labels

The next tab allows you to customize the **Labels** displayed by the
CoalaWeb Contact extension both in the forms and the sent e-mail. Note:
If your site is multilingual leave blank and use the language files.
*\[Figure-7\]*

![Figure-7](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-config-labels.png "Figure-7"){.coalaweb-docs}

### <a name="options-captcha"></a>5. Captcha

The next tab allows you to display a **Captcha** to attempt to reduce
pesky spam. Lets start with the options that apply to both the **Core**
and **Pro** versions of the extension. Firstly you have the option to
pick what type of Captcha you wish to display. The **Core** users only
get one option the basic question and answer type Captcha while **Pro**
users get three. Next you get to choose if you want to display a
title/hint above the Captcha.

#### Basic Captcha

The next two options are applicable when using the basic question and
answer type Captcha [The Default Captcha]. They allow you to chose a
question to be displayed and the answer to be check against before
allowing the form to be submitted. The default question is:

    Question = How many wheels does a bicycle have?

    Answer = 2

Feel free to choose a question and answer but try to aim for a good
balance between difficult to answer for a spam bot while not too
annoying for a real user. Note: If your site is multilingual leave blank
and use the language files. *\[Figure-8\]*

![Figure-8](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-config-captcha1.png "Figure-8"){.coalaweb-docs}

For the Pro subscribers you get two additional Captcha options.

#### Math Captcha

This is a math question and answer type Captcha here you have the option
to choose some custom text both before and after the question. Note: If
your site is multilingual leave blank and use the language files. *\[Figure 9\]*

#### ReCaptcha

<div class="alert">Note: Recaptcha can only be displayed once on a page. I'm currently looking into a reliable work around for this issue and I will implement it if one becomes available.</div>

You also get the option to use ReCaptcha which will require you to Copy
and paste your Public and Private keys in fields provided and theme you
wish to use.

To get started grab your Public and Private keys by signing in with your
Google account (create an account if you don't have one) here: [Create a
reCAPTCHA key](https://www.google.com/recaptcha/admin/create). Once you
have an account register your website domain, and Google will provide
you with your ReCaptcha keys. *\[Figure-9\]*

![Figure-9](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-config-captcha2.png "Figure-9"){.coalaweb-docs}

### <a name="options-advanced"></a>6. Advanced

In this section there is only one option to turn on or off the **Email Cloak** let me explain when to use this option. If you have disabled the native Joomla email cloak plugin or you are using a third party extension to cloak your emails please set the option below to No. *\[Figure-9b\]*

![Figure-9b](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-config-advanced1.png "Figure-9b"){.coalaweb-docs}

### <a name="options-updates"></a>7. Update Options

The CoalaWeb Contact extension integrates with the inbuilt
**Joomla Update** system so both **Core** and **Pro** users can keep their
extension up to date. For the **Pro** users you will have to copy and
paste your **Download ID** into this field to allow the update system to
work. Once you have added your **Download ID** the message displayed in
the **Control Panel** will disappear. If you try to update and it fails
make sure you still have a valid subscription and the **ID** is correct. *\[Figure-10\]*

![Figure-10](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-config-updates.png "Figure-10"){.coalaweb-docs}

### <a name="options-downloadid"></a>8. Where Is My Download ID \[Pro Version\]

To find your **Download ID** log into **coalaweb.com** and from the top
menu select **Members → My Subscriptions** scroll down and under **My
Subscriptions** there is a Module called **Download ID** now copy the
code and paste it back in your component configuration making sure not
to include any spaces. *\[Figure-11\]*

![Figure-11](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/coalaweb-download-id.png "Figure-11"){.coalaweb-docs}

### <a name="options-permissions"></a>9.Component Permissions

The last tab contains the permission settings for the CoalaWeb Contact
component. *\[Figure-12\]*

![Figure-12](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-config-permissions.png "Figure-12"){.coalaweb-docs}

# <a name="module"></a>Contact Module

![Module-Demo](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-module-themes.png "Module-Demo"){.coalaweb-docs}

### <a name="mod-general"></a>General Display Options

To make it easier to follow I have broken up the General settings into
four parts.

**Note:** The options below will override the component configuration.

#### Part 1

The first thing that will need to be filled in is the **Recipient
Email** with out this the system will display an error message. If you
have purchased a Pro subscription you will also have two more fields
available a CC Email and a BCC email option fill these in as necessary.
Next you have a **Default Subject** option this will display in the
email subject followed by the submitters subject if you have chosen to
display this option. *\[Figure-13\]*

![Figure-13](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-mod-config-general1.png "Figure-13"){.coalaweb-docs}

#### Part 2

Next we have some **Field Display** options that will affect what and how items are displayed within the contact form. Firstly you have the option to turn on or off the display of the following fields **Name**, **Subject** and **Message** and also if they are required. If you are using the **Pro** version you will also have two more options **Date From** and **Date To** these will display with a **Calendar** selector next to these fields. 

The next option gives **Pro** users the ability to display a **Terms of Service** input field that can also be set to required. Note: If you want to display the **TOS**  you will also need to enter an article **ID** in the **Component** configuration options. Next you can chose to display a **Copy Me** field allowing users to receive a copy of the form when they submit it. The last two options are for the **Pro** subscribers and they allow you to set and display the **Character Limit** for the message field of the form. If displayed the **Character Limit** will count down as text is entered into the message field. *\[Figure-14\]*

![Figure-14](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-mod-config-general2.png "Figure-14"){.coalaweb-docs}

#### Part 3

In this section you can set the **Redirection** after the mail has been successfully sent. The **Core** version gives you two options the first one is to return to the **Same Page** that the form was submitted on while the second one will return the user to the **Home Page** of your website. The **Pro** version has an additional **Custom URL** option that if chosen will redirect the user to the URL entered in the following **Custom URL** field. *\[Figure-14b\]*

![Figure-14b](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-mod-config-general2b.png "Figure-14b"){.coalaweb-docs}

#### Part 4

Lastly we have some **Layout & Style** options that will affect the look
and feel of the contact form. The first option allows you to choose a
**Theme** for the contact form. **Core** users only have one option
while the **Pro** subscribers get two.

#### Creating your own theme

Creating a theme is easy just copy the light folder found in:

    media → coalawebcontact → components → contact → themes

Give it a different name and edit as needed all the folders in the
themes folder will automatically be listed in the **Form Theme** select
list. Next you can choose the width of the contact form in %. The next
option allows you to choose a **Button Style** for the contact form.
**Core** users only have the default option while the **Pro**
subscribers get 6 color options as well. The last two options allow you
to choose the text to be displayed on the **Submit** button at the
bottom of the contact form and for the **Pro** users the button
displayed at the bottom of the editor window allowing you to insert a
form into your content. *\[Figure-15\]*

![Figure-15](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-mod-config-general3.png "Figure-15"){.coalaweb-docs}

### <a name="mod-custom"></a>Custom Fields

In this section you can choose to display one custom field for **Core** users or up to three for **Pro** users. The specifics for each custom fields can be found in the component configuration options. *\[Figure-15b\]*

![Figure-15b](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-mod-config-custom1.png "Figure-15b"){.coalaweb-docs}

### <a name="mod-captcha"></a>Captcha

The next options group allows you to display a **Captcha** to attempt to
reduce pesky spam. Lets start with the options that apply to both the
**Core** and **Pro** versions of the extension. Firstly you have the
option to pick what type of captcha you wish to display the **Core**
users only get one option the basic question and answer type Captcha
while **Pro** users get three. Next you get to chose if you want to
display a title/hint above the Captcha.

#### Basic Captcha

The next two options are applicable when using the basic question and
answer Captcha they allow you to chose a question to be displayed and
the answer to be check against before allowing the form to be submitted.
The default question is:

    Question = How many wheels does a bicycle have?

    Answer = 2

Feel free to chose a question and answer but try to aim for a good
balance between difficult to answer for a spam bot while not too
annoying for a real user. Note: If your site is multilingual leave blank
and use the language files. *\[Figure-16\]*

![Figure-16](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-mod-config-captcha1.png "Figure-16"){.coalaweb-docs}

<div class="alert">For the <em>Pro</em> subscribers you get two additional Captcha options.</div>

#### Math Captcha

This is a math question and answer type Captcha here you have the option
to chose some custom text both before and after the question. Note: If
your site is multilingual leave blank and use the language files. *\[Figure-17\]*

![Figure-17](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-mod-config-captcha2.png "Figure-17"){.coalaweb-docs}

#### ReCaptcha

<span class="alert" markdown="1">Please note Recaptcha can only be displayed once on a page. I'm
currently looking into a reliable work around for this issue and I will
implement it if one becomes available.</div>

You also get the option to use ReCaptcha which will require you to Copy
and paste your Public and Private keys into the component configuration
as well as choosing the theme you wish to use also in the component
configuration. *\[Figure 9\]*

### <a name="mod-advanced"></a>Advanced Options

The CoalaWeb Contact module also has a few of what I consider **Advanced
Options** such as the option to assign a **Unique Module ID** to stop
conflicts, a **Module Class Suffix** and whether to use **Cache**
including the **Cache Time**. The last option is whether to display a
**Link Back to CoalaWeb** as always it's appreciated but its up to you
plus you can choose what text to display next to the link. Note: If your
site is multilingual leave blank and use the language files. *\[Figure-18\]*

![Figure-18](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-mod-config-advanced.png "Figure-18"){.coalaweb-docs}

### <a name="mod-release"></a>Release Information

In this section you can find out information about the currently installed extension
such as **Type**, **Version** and **Release Date**. *\[Figure-19\]*

![Figure-19](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-mod-config-r-info.png "Figure-19"){.coalaweb-docs}

## <a name="plg"></a>Plugins \[PRO\]

### <a name="plg-content"></a>Content Plugin - Contact

The CoalaWeb Contact plugin gives you even more flexibility by allowing
you to place one or more contact forms anywhere within your content. All
of the configuration options for this particular plugin can be found in
the accompanying component under **Extension Options**. If you can't see
the contact form displayed in your content make sure you have the plugin
installed and published and that you have selected the appropriate
configuration options.

![Content-PLG-Demo](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-plg-content.png "Content-PLG-Demo"){.coalaweb-docs}

### <a name="plg-xtd"></a>Editor XTD Plugin - Contact

The **Editor XTD** plugin makes adding a contact form to your Joomla
content a one click process. Just place the cursor where you want the
form to be displayed and then click the **Insert Contact** button
displayed at the bottom of the editor.

![XTD-PLG-Button](http://cdn.coalaweb.com/images/docs/joomla-extensions/contact/cw-contact-plg-btn.png "XTD-PLG-Button"){.coalaweb-docs}

### <a name="more-help"></a>Need more help?

<div class="uk-alert">Do you have a question that wasn't covered by this GUIDE? Try the <a href="http://coalaweb.com/support/documentation/category/contact" target="_self">FAQ</a></div>

<div class="uk-alert">Do you have a question that wasn't covered by this GUIDE or the FAQ? Then it's time to drop by the <a href="http://coalaweb.com/forum/index" target="_self">Forum</a></div>
