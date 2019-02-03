## Table of Contents
1.  [Intro](#intro)
2.  [Guide](#guide)
5.  [Tips](#tips)
6.  [System Information](#system-info)
7.  [Need More Help?](#more-help)

## <a name="intro"></a>Intro

If you want to contributed to a project hosted on **GitHub** you will find the majority of the projects ask that you do it in the form of a **Pull Request**. If you want to learn more about how to submit a pull request read on.

<div class="uk-alert">Note: This guide was created using the IDE <strong>PhpStorm</strong> on a <strong>Ubuntu</strong> based machine but the fundamentals remain the same for most setups.</div>

## <a name="guide"></a>Guide

PhpStorm updates are usually patch-based: they are applied to the existing installation and only require you to restart the IDE. Due to the current limitations of the update system, these patches can only be applied sequentially, on top of one another. For example, if you are using PhpStorm 2017.1.1, you can patch it to 2017.1.2, but not to 2017.1.3.

If you skip or ignore a patch, you will lose the ability to apply the subsequent patches. As a result, when a new PhpStorm version is released, you will see a dialog box prompting you to download and install it:

ps_update_download

If this happens, you can restore the ability to apply patched-based updates by manually applying skipped updates one by one.

Follow these steps:

    Ignore the proposed update by clicking Ignore This Update. This way, you will add the proposed build’s number to the Ignored updates list.
    Open the PhpStorm Settings / Preferences dialog and navigate to Appearance and Behavior | System Settings | Updates.
    Click the Check Now button to check for available updates. If you only skipped a single update, the update dialog box will now prompt you to update and restart PhpStorm. Otherwise, keep ignoring the proposed updates until a patch-based update is proposed.
    Update and restart PhpStorm.
    Navigate back to the Updates settings page and click the View/edit ignored updates link to open the Ignored updates list.
    Delete the ignored build’s number from this list and check for available updates once more. The update that you have un-ignored will show up, and you can now apply it as a patch as well. Note that if you have ignored several updates, you need to remove and apply them one by one, starting from the oldest update.


TIP: If after you install an older pacth your click the View/edit irgnore updates link and nothing happends I found if you close settings and click Help from the top menu and then Check for updates the same in link in the pup winow would work and then for what ever reason you close the popup and go back to setting the link would also work there.

## <a name="tips"></a>Tips

 - You can check out a new project using any open PhpStorm project and don't worry it won't affect the current project just choose to open it in a new window

 - Give as much detail as possible with your pull request to help the project managers understand why you have made your changes and help then check and potential test your proposed changes.
 
 - When you have submitted your **Pull request** make sure it passes all the checks and gets a nice green tick to give it it's best chance of being accepted. *\[Figure-7\]*

<a data-lightbox="on" href="https://d1tgoab1lhw0tx.cloudfront.net/images/docs/git/pull-request/figure-7.png">![Figure-7](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/git/pull-request/figure-7.png "Figure-7"){.uk-thumbnail .uk-thumbnail-mini}</a> 

## <a name="system-info"></a>System Information

-   Git: 2.7.4
-   Ubuntu: 16.04 LTS
-   PhpStorm: 2018.2.6

## <a name="more-help"></a>Need More Help?

If you need more help or have any questions regarding this guide feel free to:

 - Start a new [forum](https://coalaweb.com/forum/index) topic if it wasn't covered by this guide
 - Send an email to support at our domain name
 - Send a tweet or a Twitter direct message to [@coalaweb](https://twitter.com/CoalaWeb)
 - Contact us through our [Facebook page](https://www.facebook.com/CoalaWeb)
 - Alternatively, you can use our [Contact Us](https://coalaweb.com/support/get-in-touch/contact-us) form