## Table of Contents
1.  [Overview](#overview)
2.  [Database Records](#database-records)
    - [Example](#db-example)
3.  [Menu Fix](#menu-fix)
4.  [File removal](#file-removal)
    - [Example](#file-example)
5.  [TMP Folder](#tmp-folder)
6.  [Need More Help?](#more-help)

## <a class="doc-top" name="overview"></a>Overview

Sometimes a component will fail to install correctly for a variety of reasons such as a server timeout, insufficient resources or a permissions issue just to name a few. Another scenario is that the system does not completely remove all the related component data while uninstalling. In cases such as these you can do it manually with the following steps.
 
### <a name="database-records"></a>Database Records
To manually remove all references to component in the database a series of SQl queries can be executed using a tool such as phpMyAdmin. Before doing this, it's important that you are familiar with the basic principals and commands of SQL.
 
<div class="uk-alert">Note: Change the <em>#__</em> to your current Joomla database prefix, e.g. #__extensions to jos_extensions</div>
  
#### <a name="db-example"></a>Example

 Here is an example for removing the database records related to the CoalaWeb Traffic component.

    -- Experienced database users only
    -- Run these queries in a database editor such phpMyAdmin
     
    -- Manual removal of CoalaWeb Traffic component from a Joomla database
    -- Change the #__ to your current Joomla database prefix
     
    DELETE FROM `#__schemas` WHERE `extension_id` = (SELECT `extension_id` FROM `#__extensions` WHERE `type` = 'component' AND `name` = 'com_coalawebtraffic');
    DELETE FROM `#__extensions` WHERE `name` = 'com_coalawebtraffic';
    DELETE FROM `#__assets` WHERE `name` = 'com_coalawebtraffic';
    DELETE FROM `#__menu` WHERE `type` = 'component' AND `title` LIKE '%com_coalawebtraffic%';
    DELETE FROM `#__session` WHERE  `data` LIKE '%com_coalawebtraffic%';

### <a name="menu-fix"></a>Menu Fix

Occasionally component menu links are not displayed in the Joomla components menu, to fix this try running these SQL queries:
 
     -- Experienced database users only
     -- Run these queries in a database editor such phpMyAdmin

    -- Manually publishing of the CoalaWeb Traffic component menu items
    -- Change the #__ to your current Joomla database prefix

    
    UPDATE `#__menu` SET `published` = '1' WHERE `type` = 'component' AND `title` LIKE '%com_coalawebtraffic%';
    UPDATE `#__menu` SET `component_id` = (SELECT `extension_id` FROM `#__extensions` WHERE `type` = 'component' AND `name` = 'com_coalawebtraffic') WHERE `type` = 'component' AND `title` LIKE '%com_coalawebtraffic%';

### <a name="file-removal"></a>File Removal

If you are removing the component manually, it is possible that some files and folders of the related component will remain on your server. In cases such as these you can connect to your server with a FTP client and delete them manually.

<div class="uk-alert">Note: Be careful not to remove any other parts of the system. I reommend that you have at least basic Joomla filesystem knowledge to make these changes.</div>

<div class="uk-alert">Note: Only ever delete the last folder in the path, for example if the path is: administrator/components/com_coalawebtraffic, you should only delete the <em>com_coalawebtraffic</em> folder.</div>
 
#### <a name="file-example"></a>Example
 
For example, if you wanted to remove the CoalaWeb Traffic component you would delete the following folders:

    components/com_coalawebtraffic
    administrator/components/com_coalawebtraffic
    media/coalawebtraffic

and these files:

    language/en-GB/en-GB.com_coalawebtraffic.ini
    language/en-GB/en-GB.com_coalawebtraffic.sys.ini
    administrator/language/en-GB/en-GB.com_coalawebtraffic.ini
    administrator/language/en-GB/en-GB.com_coalawebtraffic.sys.ini

### <a name="tmp-directory"></a>TMP Folder
 
Sometimes you may need to empty the main **tmp** folder which is normally found in root of your Joomla installation but if you are not sure of its exact location you can check by going to:

    Global Configuration -> Server Server Settings -> Path to Temp Folder
    
It only contains temporary files and folders so there shouldn't be any important data stored  here and so it's safe to be cleaned up if needed.

## <a name="more-help"></a>Need More Help

<div class="uk-alert">Do you have a question that wasn't covered by the GUIDE? Then it's time to drop by the <a href="https://coalaweb.com/forum/index" target="_self">Forum</a></div>