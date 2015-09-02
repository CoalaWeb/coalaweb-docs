## Table of Contents

1.  [Intro](#intro)
2.  [Guide](#guide)
    -   [Install](#install)
    -   [Convert](#convert)
5.  [Things to note](#notes)
6.  [Need More Help?](#more-help)

## <a name="intro"></a>Intro

What is Nautilus Image Converter? It’s an extension to mass re-size or rotate images relying on **ImageMagick’s** convert tool. 

## <a name="guide"></a>Guide

### <a name="install"></a>Install
In Ubuntu open up the software center and type **nautilus-image-converter** into the search window and you should see the package we want listed in the window. *\[Figure 1\]*

![Figure-1](http://cdn.coalaweb.com/images/docs/ubuntu/bulk-image-resize/bulk-image-resize-1.png "Figure-1"){.coalaweb-docs}

Next click install and enter your password if prompted then let Ubuntu weave its magic. Now to use this fabulous extension you will have to restart Nautilus and to do this with out having to log out open up your terminal and type:

    nautilus -q

or

    killall nautilus

If Nautilus doesn't automatically reopen try this. From the Unity menu (press the Super key) or using the run command (Alt+F2) Type in **gksudo nautilus** and then click **Run** to execute the command.

### <a name="convert"></a>Convert

Now we should have the **Nautilus Image Converter** installed and ready to use so lets navigate to the directory containing the images you wish to re-size. Next select all the images you want to re-size and **right click** you should now see two new entries in the option list **Re-size Images** and **Rotate Images**. *\[Figure 2\]*

![Figure-2](http://cdn.coalaweb.com/images/docs/ubuntu/bulk-image-resize/bulk-image-resize-2.png "Figure-2"){.coalaweb-docs}

Lets try it out by scrolling down and select **Re-size Images** You will be confronted with a re-size image options window. *\[Figure 3\]*

![Figure-3](http://cdn.coalaweb.com/images/docs/ubuntu/bulk-image-resize/bulk-image-resize-3.png "Figure-3"){.coalaweb-docs}

You have two main option the first is **Image Size** here you can choose the following methods of resizing.

-   Select a size from the predefined option list I normally use this.
-   Scale the images by percentage the default value is by 50%.
-   Select a custom size (Make sure you scale proportionally).

The next section is related to the file name given to the re-sized images if you want to keep the originals select some text to be appended to the end of each image but if don't need the originals select **Re-size in place**. When you are happy with your settings hit **Re-size** and wait to be amazed.

### All Done

You should now have a bunch of re-sized images ready to be used in what ever project you are working on.

## <a name="notes"></a>Things to note

-   Nautilus Image Converter: 0.3.1
-   Linux version: Ubuntu 14.04.2 LTS

## <a name="more-help"></a>Need More Help

<div class="uk-alert">Do you have a question that wasn't covered by this GUIDE? Then it's time to drop by the <a href="http://coalaweb.com/forum/index" target="_self">Forum</a></div>