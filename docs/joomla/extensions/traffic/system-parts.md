## Table of Contents
1.  [Overview](#overview)
2.  [Component](#component)
3.  [Modules](#modules)
    -   [Traffic](#mod-traffic)
4.  [Plugins](#plugins)
    -   [System - Traffic Count](#plg-count)
    -   [System - Traffic Clean](#plg-clean)
    -   [System - Traffic Online](#plg-online)

## <a name="overview"></a>Overview

CoalaWeb Traffic is a Joomla 2.5 & 3.+ extension to help you keep track of the visitors to your site. You can choose to display the module and let visitors see and be amazed by your traffic or unpublish the module and view your website statistics in the **Admin** area its up to you.

<div class="uk-alert" markdown="1">When you install a CoalaWeb extension all the parts of the system will be installed at the same time making installing, 
upgrading and uninstalling a breeze.</div>

## <a name="component"></a>Component

The Component makes setting up the system plugins a breeze as well as seeing in depth visitor information, Geo location options, export reports and much more.

## <a name="modules"></a>Modules

### <a name="mod-traffic"></a>Traffic

The Module gives you the option to display your websites traffic to other visitors with a tonne of configuration options to help integrate it into your website.

## <a name="plugins"></a>Plugins

### <a name="plg-count"></a>System - CW Traffic Count

This plugin is crucial to functionality of the system it quietly counts the visits to your site and then records them in the database. It allows you to count the traffic to your site even with the module unpublished and also ensures all traffic is record regardless of the part of the site that they visit.

This plugin also takes care of blocking visitors from being counted based on your setting in the CoalaWeb Traffic component.

### <a name="plg-clean"></a>System - CW Traffic Clean

This plugin carries out the automatic database clean up but only if you have it turned on in the Component Options. It will run in the background keeping the current data but delete out the old entries and then add them to a running total. It is recommended to turn this feature on.

### <a name="plg-online"></a>System - CW Traffic Online

This plugin will count and then supply the information so the Traffic module can display the currently online visitors. It uses it own database table along with cookies to keep track of visitors.