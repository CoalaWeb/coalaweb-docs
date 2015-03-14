## Table of Contents

1.  [Intro](#intro)
2.  [Guide](#guide)
    -   [Per Project](#project)
    -   [Globally](#global)
5.  [Things to note](#notes)
6.  [Need More Help?](#more-help)

## <a name="intro"></a>Intro

Git has two kinds of config files that affect what is set for the default **author/commiter**.

## <a name="guide"></a>Guide

### <a name="project"></a>Per Project

The first is the local **config** file which can be found in each of the projects that you have set up with git. The default location for a **Netbeans** project would be something like this:

    ~/NetBeansProjects/example-project/.git

<div class="uk-alert">Note: The <em>~/</em> is the short form for your <em>home/username</em> directory</div>

Below is an example of a  typical project config file which you might note is missing a reference to a user which means the system will look elsewhere for this info.

    [core]
        repositoryformatversion = 0
        filemode = true
        logallrefupdates = true
        bare = false
    [remote "origin"]
        url = https://example@github.com/example/example-project.git
        fetch = +refs/heads/*:refs/remotes/origin/*
    [branch "extended-version"]
        remote = origin
        merge = refs/heads/extended-version
    [pack]
        buildbitmaps = false

If we wanted to set the default **Author** and **Commiter** for this particular project all we need to do is amend this to the end:

    [user]
        name = Your Name
        email = your@email.com

<div class="uk-alert">Note: Remember this file only affects the repository it is stored in.</div>

Now if you open your project and attempt a commit the Author and Commiter should be automatically populated with the info you just added to the config file. If you are looking for a solution that will affect all your projects in one go continue reading.

### <a name="global"></a>Globally

The second is the **global user-wide** config file that affects all your repositories. This is the place where you set your primary name and email. 

The default location for the global Git config file should be here:

     ~/.gitconfig

If it does not exist feel free to create it in my case I will create it with the terminal. I find the easiest way to do this is to ask the terminal editor **Nano** to open the file and if it exists is will open it if it doesn't it will still open a editor window and when I save it will create it for me. To get started open a terminal window and type:

    sudo nano ~/.gitconfig


Enter your password to gain root privileges and you should now be confronted with a terminal editor so all you have to do is add your user details as mentioned earlier. *\[Figure 1\]*

![Figure-1](http://cdn.coalaweb.com/images/docs/git/default-git-user/default-git-user-2.png "Figure-1"){.coalaweb-docs}

To save and exit just hit **ctrl x** then for the first question choose **y** and next click **enter** *\[Figure 2\]*

![Figure-2](http://cdn.coalaweb.com/images/docs/git/default-git-user/default-git-user-3.png "Figure-2"){.coalaweb-docs}

For the last question just hit **enter** *\[Figure 3\]*

![Figure-3](http://cdn.coalaweb.com/images/docs/git/default-git-user/default-git-user-4.png "Figure-3"){.coalaweb-docs}

If you want you can check the file was created with the right content by just using Nano. Open the file again as we did in the first step and once you are happy hit **ctrl x**. If you leave without making any changes it will automatically drop out of the editor window.

### All Done

That should be it, now when committing both the **Author** and **Commiter** should be auto populated with your chosen details.

## Things to note

-   Git version 1.9.1
-   Linux version: Ubuntu 14.04.2 LTS
-   Netbeans version: 8.0.2
-   Nano version: 2.2.6

## <a name="more-help"></a>Need More Help

<div class="uk-alert">Do you have a question that wasn't covered by this GUIDE? Then it's time to drop by the <a href="http://coalaweb.com/forum/index" target="_self">Forum</a></div>