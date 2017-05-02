## Table of Contents
1.  [Intro](#intro)
2.  [Create API Key](#create)
4.  [Need More Help?](#more-help)

## <a class="doc-top" name="intro"></a>Intro

After about 10 years of allowing keyless use Google Maps as of the 22nd of June 2016 has started requiring an API key. If you have started using Google Maps on or after that date then you will need to sign up for and create a free API key.

<div class="uk-alert">Note: Older users still do not need an API key so you can try without one first if you like.</div>

Before we get started I would like to point out that the Google API interface does appeared to be geared towards developers so it can be a bit confusing for the average user. Having said that if you follow the steps covered in this guide you should be up and running in no time.

## <a name="Create"></a>Create a Google Maps API Key

Following the steps outlined below to create and implement a free [Google Maps API Key]( https://developers.google.com/maps/documentation/javascript/get-api-key)

1. Start Google’s [Get a Key](https://console.developers.google.com/flows/enableapi?apiid=maps_backend,static_maps_backend,geocoding_backend,directions_backend,distance_matrix_backend,elevation_backend,roads,street_view_image_backend,maps_embed_backend,places_backend,geolocation,timezone_backend,maps_android_backend,maps_ios_backend,placesandroid,placesios&keyType=CLIENT_SIDE&reusekey=true) process and then log into your Google account (or create a new one).

2. Click **Agree and continue** to create a new project for your specific website. *\[Figure-1\]*

![Figure-1](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/contact/api-key/cw-api-key-figure1.png "Figure-1"){.coalaweb-docs}

3. Under **Accept requests**, add the two entries below (replacing yourname.com with your own domain). Type the first entry then hit enter on your keyboard to add it. Repeat to add the second entry. Having both entries (with asterisks) will help ensure your maps work on any URL related to your website.  *\[Figure-2\]*

    yourname.com/*
    *.yourname.com/*

![Figure-2](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/contact/api-key/cw-api-key-figure2.png "Figure-2"){.coalaweb-docs}

4. Click **Create** and then **Copy** your newly created key that will display in the next screen. *\[Figure-3\]*

![Figure-3](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/contact/api-key/cw-api-key-figure3.png "Figure-3"){.coalaweb-docs}

5. Now you have your new API Key it's time to use it by pasting it into the **API Key** field found in the CoalaWeb Contact **Component Options** under the **Map** tab. *\[Figure-4\]*

![Figure-4](https://d1tgoab1lhw0tx.cloudfront.net/images/docs/joomla-extensions/contact/api-key/cw-api-key-figure4.png "Figure-4"){.coalaweb-docs}

<div class="uk-alert">Note: Google claims it can take up to 5 minutes for your key to become active but I have heard reports of it taking 30 minutes or longer so please be patient if your map doesnt display right away.</div>

## <a name="more-help"></a>Need More Help

<div class="uk-alert">Do you have a question that wasn't covered by this GUIDE? Try the <a href="https://coalaweb.com/support/documentation/category/contact" target="_self">FAQ</a></div>

<div class="uk-alert">Do you have a question that wasn't covered by this GUIDE or the FAQ? Then it's time to drop by the <a href="https://coalaweb.com/forum/index" target="_self">Forum</a></div>