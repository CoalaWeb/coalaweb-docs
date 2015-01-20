## Table of Contents
1.  [Can I install CoalaWeb Social Links on multiple domains?](#q1)
2.  [Can I keep using CoalaWeb Social Links when my subscription runs out?](#q2)
3.  [Can I remove the Powered by CoalaWeb from the module?](#q3)
4.  [Can I change the images used in module?](#q4)
5.  [I'm having problems validating my webiste with W3C what can I do?](#q5)

### <a name="q1"></a>Can I install CoalaWeb Social Links on multiple domains?

**YES** - You can install Social Links on as many domains as you want. There is no domain check or restriction.

***

### <a name="q2"></a>Can I keep using CoalaWeb Social Links when my subscription runs out?

**YES** - If you have purchased a CoalaWeb PRO subscription, you have access to PRO downloads, updates and support for the length of the subscription. After it has run out you can keep using the version you have installed. However, you will no longer be able to update to a newer versions or receive support. Of course you can renew your subscription to gain access again or you can choose to downgrade to the FREE version its up to you.

***

### <a name="q3"></a>Can I remove the Powered by CoalaWeb from the module?

**YES** - You can turn the link off in the Free or Pro versions by opening up the module configuration and its under **Advanced Options -> Display link to author**.

***

### <a name="q4"></a>Can I change the images used in module?

**YES** - Creating a theme is easy, just copy the custom-example folder found in:

`media → coalawebsocial → components → sociallinks → themes-icon`

Give the theme a different name, edit the files as needed and of course add your custom icons. All the folders located in the themes-icon directory will automatically be listed in the Icon Styles select list.

***

### <a name="q5"></a>I'm having problems validating my webiste with W3C what can I do?

Each social network handles there formatting differently but the majority of them are now pushing towards HTML5 but below I have included some exceptions and know issues.

#### Joomla using HTML5

**Linkedin:**

> The text content of element script was not in the required format: Expected space, tab, newline, or slash but found l instead.

This is due to Linkedin placing a language reference such as this lang:en_GB inside the script tags.

**Stumbleupon:**

> Element name su:badge cannot be represented as XML 1.0. Element su:badge not allowed as child of element div in this context. (Suppressing further errors from this subtree.)

This is due to StumbleUpon not support HTML 5 as of yet I have included a link below outining this issue.
[StumbleUpon and HTML5](https://getsatisfaction.com/stumbleupon_help_center/topics/stumbleupon_button_does_not_validate_for_html5_w3c)

#### Joomla using XHTML 1.0 Transitional

> There is no attribute X

Any data attributes such as data-href wont pass as they are designed for HTML5 but they work fine just be aware

Now StumbleUpon will cause the following errors:

*   element "su:badge"
*   undefined there is no attribute "location"
*   there is no attribute "layout"

These won’t affect the functionality of the button but I have yet to find a solid solution but I will keep looking.

<span class="info" markdown="1">I will continue to implement changes with each new release as solutions become available.</span>

***