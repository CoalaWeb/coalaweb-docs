## List of Questions
1.  [Fatal error: Class 'JControllerLegacy' not found \[J2.5\]](#q1)
2.  [Fatal error: Class CoalawebtrafficViewControlpanel cannot extend from interface JView \[J3.+\]](#q2)
3.  [I cannot locate the field to adjust the time zone. Is this field available? \[J2.5/J3.+\]](#q3)
4.  [Manual GEO upload but com_coalawebtraffic folder empty? \[J2.5/J3.+\]](#q4)
5.  [Module not displaying correctly after update to V0.1.8 \[J2.5/J3.+\]](#q5)

***

#### <a name="q1"></a>Fatal error: Class 'JControllerLegacy' not found

Updating Joomla to the latest version will fix this issue. Legacy is a new concept that is mainly used in Joomla 3.0 but also works in the latest 2.5 releases.

Anyone with issue please check your Joomla version under Site/System Information and make sure it's the version below or newer.

`Joomla! 2.5.9 Stable [ Ember ] 4-February-2013 14:00 GMT Joomla Platform 11.4.0 Stable [ Brian Kernighan ] 03-Jan-2012 00:00 GMT`

***

#### <a name="q2"></a>Fatal error: Class CoalawebtrafficViewControlpanel cannot extend from interface JView

I think you might have installed the 2.5 version instead of the 3.0 version try uninstalling your current installation (Note: Just uninstall the component and it will take care of the other parts of the extension). Then download and install the version with J30 in the name for example

`com_coalawebtraffic-j30-0.1.5-core.zip`

***

#### <a name="q3"></a>I cannot locate the field to adjust the time zone. Is this field available?

The time zone is based on your Joomla installation's "Server Time Zone" which can be found under:

`Site -> Global Configuration -> Server or User settings`

### Instructions

1.  Login to your Joomla back-end (yoursite.com/administrator).
2.  Select "Site" then go to "Global Configuration" from the top menu.
3.  Next select "Server" from the toolbar menu.
4.  Now under "Location Settings" choose your "Server Time Zone" from the drop down menu.
5.  Lastly click "Save".

***

#### <a name="q4"></a>Manual GEO upload but com_coalawebtraffic folder empty?

I think you might be looking in the wrong location can you check again because if the directory:

`administrator/components/com_coalawebtraffic`

If this directory is empty then the component wouldn't be functioning at all. I'm 99% sure you are looking in the front end location which is:

`components/com_coalawebtraffic` 

<span class="info" markdown="1">Note: This directory will be empty as there are no front end views for CoalaWeb Traffic.</span>

Once you have found the right location it should have files similar to this including the assets directory. *\[Figure-1\]*

![Figure-1](http://cdn.coalaweb.com/images/docs/joomla-extensions/traffic/faq/cw-traffic-faq-geo-1.png "Figure-1"){.coalaweb-docs}

Then I recommend using the updated [Guide](/support/documentation/category/extensions) and follow the steps exactly.

***

#### <a name="q5"></a>Module not displaying correctly after update to V0.1.8

This is due to a restructure where some of the options were moved from the module to the component. This was because there are now statistics displayed in the backend that rely on these setting as well as the front end module.

This should be an easy one to fix:

1.  Open up the save the **Component** and **Module** Configuration Options
2.  Then clear your Joomla + Browser Cache.

***