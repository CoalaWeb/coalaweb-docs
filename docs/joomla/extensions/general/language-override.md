## Table of Contents
1.  [Intro](#intro)
2.  [Terminology](#terms)
3.  [Scenario](#scenario)
4.  [Override](#override)
    -   [Constant Known](#known)
    -   [Constant Not Known](#notknown)
5.  [Need More Help?](#more-help)

## <a class="doc-top" name="intro"></a> Intro

In this guide I will show you how to create a language override for a multi lingual site. It will be using the **CoalaWeb Contact** extension as an example and more specifically the custom input field option.

Depending on what version of CoalaWeb Contact you are using you will have one or more custom fields. If you have a single language site you could use the inbuilt component options to change it's label and associated messages but for a multi lingual site its a bit more complicated.

## <a name="terms"></a> Terminology

<div class="uk-alert">Before you start creating language overrides it's important to know a few terms that will be used when talking about language strings.</div>

Contained inside each of the language files used through out a Joomla website are a series of language strings. Each of these strings are made up of two elements a **Constant** the reference to the language string which comes first and is in capitals.

    COM_CWCONTACT_LABEL_CUSTOM1

The second part if the **Value** which will change depending on the particular language of the file in question.

    Custom 1

When we deal with language overrides the system will take care of formating the **Constant** and **Value** together for us but just for your own knowledge if you were to open a language file they would be display like this:

    COM_CWCONTACT_LABEL_CUSTOM1="Custom 1"

## <a name="scenario"></a> Scenario

I want to change the **Custom 1** field in my contact form to **Phone Number** and I have a website with both **English** and **Spanish**. To do this I will be updating the custom field's label. *\[Figure-1\]*

![Figure-1](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/general/lang-override/image-1.png "Figure-1"){.coalaweb-docs}

The **Constant** that we will be applying the override to is:

    COM_CWCONTACT_LABEL_CUSTOM1

## <a name="override"></a> Override

To get started log into the backend of your site and then go to:

    Extensions -> Language(s)

### <a name="known"></a> Constant Known 

Next select **Overrides** from the side menu. For this example I want to create a language override for **Spanish** and it will be applied to **Administrator** because thats where the language strings are stored in this case. 

<div class="uk-alert">Note: We will also make sure it is applied to the front end in a future step.</div>

To get started I first select **Spanish (español) - Administrator** from the bottom left menu and then **New** from the top menu. *\[Figure-2\]*

![Figure-2](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/general/lang-override/image-2.png "Figure-2"){.coalaweb-docs}

Next enter the **Language Constant** to be overridden. *\[Figure-3\]*

    COM_CWCONTACT_LABEL_CUSTOM1

![Figure-3](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/general/lang-override/image-3.png "Figure-3"){.coalaweb-docs}

Next enter the text to be displayed instead of the original text.  *\[Figure-4\]*

![Figure-4](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/general/lang-override/image-4.png "Figure-4"){.coalaweb-docs}

Next tick the **For both locations** option because although the language string is stored in the **Administrator** language location we want it to be applied to the **Site** part where the module is displayed. *\[Figure-5\]*

![Figure-5](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/general/lang-override/image-5.png "Figure-5"){.coalaweb-docs}

Now after you save your new override it will be displayed in the list of **Spanish (español) - Administrator** and **Spanish (español) - Site** overrides .

Now try refreshing your site to see the contact form with its new label in action. *\[Figure-6\]*

![Figure-6](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/general/lang-override/image-6.png "Figure-6"){.coalaweb-docs}

<div class="uk-alert">Note: You would also have to repeat the process for the other two associated language strings.</div>

    COM_CWCONTACT_CUSTOM1_HINT
    COM_CWCONTACT_MSG_CUSTOM1_MISSING

### <a name="notknown"></a> Constant Not Known

In this case it gets a bit more complicated because the language file that contains the **Constant** and **Value** that I want to override is **English - Administrator** and the override will need to be applied to **Spanish**. Now to find out the correct **Constant** we will first select **English - Administrator** from the side menu and then **New** from the top menu. *\[Figure-7\]*

![Figure-7](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/general/lang-override/image-7.png "Figure-7"){.coalaweb-docs}


Now I'm not sure what the exact language **Constant** is so I'm going to use the search option to the right. For example if I wanted to see what the **Constant** for the **Custom 1** label is I could set the **Search For** option to **Value** and then type **Custom 1** in the search field and click search.  *\[Figure-8\]*

![Figure-8](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/general/lang-override/image-8.png "Figure-8"){.coalaweb-docs}

In most cases you will have to have a look through the returned option to get the exact one you are looking for. *\[Figure-9\]*

![Figure-9](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/general/lang-override/image-9.png "Figure-9"){.coalaweb-docs}

Now that we have our **Constant** we can select **Spanish (español) - Administrator** from the bottom left menu and then **New** from the top menu. *\[Figure-10\]*

<div class="uk-alert">Note: We will also make sure it is applied to the front end in a future step.</div>

![Figure-10](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/general/lang-override/image-2.png "Figure-10"){.coalaweb-docs}

Next enter the **Language Constant** to be overridden. *\[Figure-11\]*

    COM_CWCONTACT_LABEL_CUSTOM1

![Figure-11](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/general/lang-override/image-3.png "Figure-11"){.coalaweb-docs}

Next enter the text to be displayed instead of the original text.  *\[Figure-12\]*

![Figure-12](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/general/lang-override/image-4.png "Figure-12"){.coalaweb-docs}

Next tick the **For both locations** option because although the language string is stored in the **Administrator** language location we want it to be applied to the **Site** part where the module is displayed. *\[Figure-13\]*

![Figure-13](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/general/lang-override/image-5.png "Figure-13"){.coalaweb-docs}

Now after you save your new override it will be displayed in the list of **Spanish (español) - Administrator** overrides.

Now try refreshing your site to see the contact form with its new label in action.  *\[Figure-14\]*

![Figure-14](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/general/lang-override/image-6.png "Figure-14"){.coalaweb-docs}

<div class="uk-alert">Note: You would also have to repeat the process for the other two associated language strings.</div>

    COM_CWCONTACT_CUSTOM1_HINT
    COM_CWCONTACT_MSG_CUSTOM1_MISSING

## <a name="more-help"></a>Need More Help

<div class="uk-alert">Do you have a question that wasn't covered by this GUIDE? Then it's time to drop by the <a href="https://coalaweb.com/forum/index" target="_self">Forum</a></div>
