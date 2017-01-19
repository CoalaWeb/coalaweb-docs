## Table of Contents

1.  [Intro](#intro)
2.  [Guide](#guide)
3.  [Tips](#tips)
4.  [Need More Help?](#more-help)

## <a name="intro"></a>Intro

> Invalidating objects removes them from CloudFront edge caches.

All your files stored on CloudFront are cached allowing them to be served as fast as possible. What if you want to update a file or image that you have stored there? You can update as many files as you like but it can take up to 24 hours for the changes to catch up. 

### Scenario

I use CloudFront to store the update files for my extensions and I can't version their names because they would stop working. To get around this every time I release a new version I manually invalidate the extensions update **xml** file using the follow procedure. 

## <a name="guide"></a>Guide

### Step 1 

First make sure you are logged into AWS and then select the **Console Home** icon from the top left. *\[Figure 1\]*

![Figure-1](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/aws/cf-invalidations/cf-invalidations-1.png "Figure-1"){.coalaweb-docs}

### Step 2

Now select **CloudFront** from the list of services. *\[Figure 2\]*

![Figure-2](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/aws/cf-invalidations/cf-invalidations-2.png "Figure-2"){.coalaweb-docs}

### Step 3

In the next window make sure you have **Distributions** selected from the top left. *\[Figure 3\]*

![Figure-3](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/aws/cf-invalidations/cf-invalidations-3.png "Figure-3"){.coalaweb-docs}

### Step 4

Next click the link for the associated distribution from the list **(under id)**. *\[Figure 4\]*

![Figure-4](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/aws/cf-invalidations/cf-invalidations-4.png "Figure-4"){.coalaweb-docs}

### Step 5

Select the **Invalidations** tab. *\[Figure 5\]*

![Figure-5](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/aws/cf-invalidations/cf-invalidations-5.png "Figure-5"){.coalaweb-docs}

### Step 6

Click the **Create Invalidation** button and then enter the location of the file/s you want to be invalidated. *\[Figure 6\]*

**For example:**

![Figure-6](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/aws/cf-invalidations/cf-invalidations-6.png "Figure-6"){.coalaweb-docs}

### Step 7

Then click the **Invalidate** button and you should now see **InProgress** under status. *\[Figure 7\]*

![Figure-7](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/aws/cf-invalidations/cf-invalidations-7.png "Figure-7"){.coalaweb-docs}

> It usually takes 10 to 15 minutes to complete your invalidation request, depending on it's size..

### Finished

Once it says completed you are good to go.

## <a name="tips"></a>Tips

### Copy previous invalidation

Once you have created a few invalidations if you come back and need to invalidate the same files try this. Click the select box for the item you want to duplicate, once you have done this the **Copy** button at the top will become available. Click the **Copy** button make any needed changes and you are done. *\[Figure 8\]*

![Figure-8](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/aws/cf-invalidations/cf-invalidations-8.png "Figure-8"){.coalaweb-docs}

## <a name="more-help"></a>Need More Help

<div class="uk-alert">Do you have a question that wasn't covered by this GUIDE? Then it's time to drop by the <a href="http://coalaweb.com/forum/index" target="_self">Forum</a></div>
