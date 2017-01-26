## Change Log

### Version 1.1.0 January 2017

#### Component - Traffic
- **(C)** City and country counts now check for non empty or NULL values
- **(A)** New GEO refresh option \[Pro\]
- **(L)** New and updated language strings

#### Plugin(S) - Gears
- **(C)** Updated to version 0.3.1

### Version 1.0.9 January 2017

#### Component - Traffic
- **(C)** Updated all Core V1 GEO database system files
- **(C)** Improved V1 GEO data retrieval and storing
- **(C)** Improved validation of GEO data retrieval
- **(C)** Updated copyright to 2017

#### Module - Traffic
- **(C)** Updated copyright to 2017

#### Module - Traffic Pro
- **(C)** Updated copyright to 2017

#### Plugin(S) - Traffic Count
- **(C)** Updated copyright to 2017

#### Plugin(S) - Traffic Online
- **(C)** Updated copyright to 2017

#### Plugin(S) - Traffic Clean
- **(C)** Updated copyright to 2017

#### Plugin(S) - Gears
- **(C)** Updated to version 0.2.9

### Version 1.0.8 December 2016

#### Component - Traffic
- **(B)** Fixed auto DB clean up system
- **(C)** Fixed OVH server IP detection
- **(A)** New option to store DB errors in a log file
- **(A)** New option to store DEBUG info in a log file
- **(A)** Integrated new DEBUG log option into iptools helper file
- **(A)** Display Pro fields in core version
- **(A)** 6 new Robots added to auto populate list \[Pro\]
- **(L)** New and updated language strings

#### Module - Traffic
- **(A)** Integrated new DB log option for all queries
- **(A)** Display Pro fields in core version
- **(L)** New and updated language strings

#### Module - Traffic Pro
- **(A)** Integrated new DB log option for all queries
- **(A)** Added custom CSS file option
- **(L)** New and updated language strings

#### Plugin(S) - Traffic Count
- **(A)** Integrated new DB log option for all queries

#### Plugin(S) - Traffic Online
- **(A)** Integrated new DB log option for all queries

#### Plugin(S) - Traffic Clean
- **(B)** Fixed auto DB clean up system
- **(A)** Integrated new DB log option for all queries

### Version 1.0.7 November 2016

#### Component - Traffic
- **(B)** Fixed missing framework call in Known IP edit

### Version 1.0.6 October 2016

#### Component - Traffic
- **(C)** formvalidation is depreciated and replaced with formvalidator
- **(C)** Complete rewrite of the GEO upload and install system
- **(C)** Now using GEO databases with their original names
- **(C)** Updated helper class checks
- **(A)** GEO database renaming function for retro compatibility
- **(A)** 6 new Robots added to auto populate list \[Pro\]
- **(L)** New and updated language strings

#### Module - Traffic Pro
- **(A)** Max displayed flags option
- **(L)** New and updated language strings

#### Plugin(S) - Traffic Clean
- **(B)** Database cleanup done in 50 record chunks to keep queries fast

#### Plugin(S) - Gears
- **(C)** Updated to version 0.2.6

### Version 1.0.5 September 2016

#### Component - Traffic
- **(C)** New proxy check option for Iptools class

### Version 1.0.4 August 2016

#### Component - Traffic
- **(C)** Iptools class has improved IP detection and validation

#### Plugin(S) - Traffic Count
- **(B)** Fixed issue with known IP blocking

### Version 1.0.3 August 2016

#### Component - Traffic
- **(C)** Referer check in visitors view
- **(C)** Iptools class has improved IP detection and validation

#### Plugin(S) - Traffic Count
- **(C)** Improved validation of HTTP_REFERER 

### Version 1.0.2 August 2016

#### Component - Traffic
- **(B)** Fixed discrepancy with date and time in CSV report
- **(C)** GEO install tmp directory check
- **(C)** Iptools class fix for when HTTP_X_FORWARDED_FOR contains multiple IPs

#### Plugin(S) - Gears
- **(C)** Updated to version 0.2.5

### Version 1.0.1 June 2016

#### Component - Traffic
- **(B)** Fix untranslated strings in Visitor view
- **(C)** Control panel statistics code improvements
- **(C)** Code improvements in Visitor view
- **(C)** GEO upload and unzip merged into one step
- **(C)** GEO install attempts to temporarily increase PHP limits while installing 
- **(C)** GEO install layout improvement
- **(C)** Improved error checking when using the GEO database
- **(C)** Purge now uses truncate to re-index after deletion
- **(A)** GEO one click update cpanel button \[Pro\]
- **(A)** New manage view
- **(A)** New database backup option \[Pro\]
- **(A)** New database restore option \[Pro\]
- **(A)** Release information displays latest release

#### Admin Module - Traffic Stats \[Pro\]
- **(N)** Integrated into the CoalaWeb Traffic extension

#### Plugin(S) - Gears
- **(C)** Updated to version 0.2.3

### Version 1.0.0 May 2016

#### Component - Traffic
- **(B)** Fix missing column error when filtering visitors
- **(B)** Check definitions in geoip.inc
- **(C)** Changed mb_substr for JString::substr
- **(C)** Added graceful message for if helper files are missing
- **(C)** Updated copyright date to 2016
- **(C)** New styling for Tabs, Tables and Control Panel
- **(C)** Using JApplicationWebClient for Browser/Platform and User Agent info
- **(C)** Changed JError to JLog for install script notices
- **(C)** Rewritten control panel and geo updates
- **(C)** Complete code clean up and improvements
- **(C)** Changed JArrayHelper for ArrayHelper
- **(R)** Removed Joomla 2.5 support
- **(R)** Removed old Browser/Platform class
- **(R)** Removed obsolete options
- **(R)** Removed filter CSV export option
- **(R)** Removed old system transfer code from install scripts
- **(A)** Catching DB errors
- **(A)** New charts system (Pro)
- **(A)** Incorporated Geo V2 (Pro)
- **(A)** Simple bot blocking using JApplicationWebClient (Pro)
- **(A)** New purge database option
- **(A)** New repair and optimize database option (Pro)
- **(A)** New import robots list (Pro)
- **(A)** New option to not store IP in raw format (Pro)
- **(A)** New store location option (Pro)
- **(A)** New Detect class for interpreting Browser and Platform names
- **(L)** Rewritten control panel and GEO updates
- **(L)** New and updated language strings
- **(L)** Fixed missing language strings

#### Module - Traffic
- **(C)** Updated copyright date to 2016
- **(C)** Added graceful message for if helper files are missing
- **(C)** Using JApplicationWebClient for Browser/Platform and User Agent info
- **(R)** Removed Joomla 2.5 support
- **(R)** Removed author support links
- **(R)** Removed old Browser/Platform class
- **(A)** Incorporated Geo V2 (Pro)
- **(A)** Option to turn off Core CSS (Pro)
- **(A)** Option to included custom CSS file (Pro)
- **(L)** New and updated language strings

#### Module - Traffic Pro
- **(N)** Integrated into the CoalaWeb Traffic extension

#### Plugin(S) - Traffic Count
- **(B)** Fixed undefined index when no HTTP_USER_AGENT 
- **(C)** Using $db->execute(); for Joomla 3.+
- **(C)** Added graceful message for if helper files are missing
- **(C)** Using JApplicationWebClient for Browser/Platform and User Agent info
- **(C)** Using CoalaWebBot class for basic identification (Pro)
- **(C)** Integrated new IP stored as hash
- **(C)** Stores GEO data while saving visitor info
- **(C)** Updated copyright date to 2016
- **(R)** Removed Joomla 2.5 support
- **(R)** Removed old Browser/Platform class
- **(A)** Catching DB errors
- **(A)** Incorporated Geo V2 (Pro)

#### Plugin(S) - Traffic Online
- **(B)** Fixed undefined index when no HTTP_USER_AGENT
- **(C)** Added graceful message for if helper files are missing
- **(C)** Using JApplicationWebClient for Browser/Platform/Bot and User Agent info
- **(C)** Updated copyright date to 2016
- **(R)** Removed Joomla 2.5 support
- **(R)** Removed old Browser/Platform class
- **(A)** Catching DB errors
- **(A)** Incorporated Geo V2 (Pro)

#### Plugin(S) - Traffic Clean
- **(C)** Updated copyright date to 2016
- **(C)** Only executed on front end
- **(R)** Removed Joomla 2.5 support
- **(A)** Catching DB errors

#### Plugin(S) - Gears
- **(C)** Updated to version 0.2.2

### Version 0.1.9 February 2015

#### Component - Traffic
- **(C)** Combined all the change logs into one.
- **(C)** Updated install script.
- **(A)** Added new export all report option.
- **(B)** Fixed honey pot blocking bug.
- **(B)** Fixed display of Known IP info in visitors view.
- **(L)** Added new language strings.
- **(L)** Updated some language strings.
- **(C)** Change Browser class name to stop potential conflicts.

#### Module - Traffic
- **(B)** Fixed doubled advanced tab in module configuration.
- **(C)** Overhauled horizontal and compact layouts.
- **(A)** Added digital counter to all layouts.
- **(A)** Horizontal and Compact digital display option.
- **(C)** Expanded horizontal text option.
- **(A)** 3 new digital counter sizes for each theme.
- **(L)** Added new language strings.
- **(L)** Updated some language strings.
- **(C)** Change Browser class name to stop potential conflicts.

#### Module - Traffic Pro \[Pro\]
- **(N)** Integrated into CoalaWeb Traffic extension.

#### Plugin(S) - Traffic Count
- **(B)** Fixed honey pot blocking bug.
- **(C)** Change Browser class name to stop potential conflicts.

### Version 0.1.8 May 2014

#### Component - Traffic
- **(A)** Back end counter statistics.
- **(A)** Added Known IP categories.
- **(C)** Overhauled the Known IP system to included the ability to block IPs and Bots + more.
- **(A)** 4 new visitor attributes saved and displayed.
- **(A)** Project Honey integration.
- **(A)** 4 new clean up database options.
- **(A)** Week start on Sunday option.
- **(A)** Integration of the CoalaWeb Gears framework plugin.
- **(C)** Merged 2.5 and 3.2 versions into one package.
- **(B)** Various bug fixes and improvements.
- **(C)** Geo Data system checks if already installed.
- **(A)** New fall back to English language system if string is unavailable.

#### Module - Traffic
- **(A)** New digit style counter.
- **(A)** 2 digit counter styles.
- **(C)** Totally updated default module layout.
- **(C)** Totally overhauled module icon theme system.
- **(C)** New method for detecting the visitors information.
- **(A)** New who is online plugin that uses cookies.
- **(A)** New section system to allow complete control over what gets displayed.
- **(A)** Integrated CoalaWeb Gears framework plugin.
- **(B)** Various bug fixes and improvements.
- **(C)** Merged 2.5 and 3.2 versions into one package.
- **(A)** New fall back to English language system if string is unavailable.

#### Plugin(S) - Traffic Count
- **(A)** New method for identifying IPs.
- **(A)** New system for blocking IPs and Bots.
- **(A)** Integrated Project Honeypot.
- **(A)** Now capturing browser, operating system and referral  info.
- **(A)** Integrated CoalaWeb Gears framework plugin.
- **(B)** Various bug fixes and improvements.
- **(C)** Merged 2.5 and 3.2 versions into one package.
- **(A)** New fall back to English language system if string is unavailable.

#### Plugin(S) - Traffic Clean
- **(A)** New options for when to clean up.
- **(A)** Integrated CoalaWeb Gears framework plugin.
- **(B)** Various bug fixes and improvements.
- **(C)** Merged 2.5 and 3.2 versions into one package.
- **(A)** New fall back to English language system if string is unavailable.

#### Plugin(S) - Traffic Online
- **(N)** Integrated into the system

### Version 0.1.7 June 2013

#### Component - Traffic
- **(B)** Fixed menu icon link.
- **(C)** Updated help URL.

#### Module - Traffic
- **(C)** Updated who is online to only display Guests/Members from the last 10 minutes.
- **(C)** Updated helper file to work for both 2.5 and 3.+.

#### Plugin(S) - Traffic Count
- **(C)** Updated code to work for both 2.5 and 3.+

#### Plugin(S) - Traffic Clean
- **(B)** Fixed clean up bug.
- **(C)** Updated code to work for both 2.5 and 3.+

### Version 0.1.6 May 2013

#### Component - Traffic
- **(C)** CSS tweak.

### Version 0.1.5 April 2013

#### Component - Traffic
- **(C)** New Name: CoalaWeb Traffic
- **(C)** Expanded minimum geo upload requirements check.
- **(A)** Add info links to IP's listed as visitors.
- **(C)** Updated and expanded administrator CSS.
- **(A)** New language strings.
- **(B)** Fixed potential language bug.
- **(A)** Added two new custom fields to style configuration screens.

#### Module - Traffic
- **(C)** New Name: CoalaWeb Traffic
- **(C)** Default css updates.

#### Plugin(S) - Traffic Count
- **(C)** New Name: CoalaWeb Traffic

#### Plugin(S) - Traffic Clean
- **(C)** New Name: CoalaWeb Traffic

### Version 0.1.4 March 2013

#### Component - Traffic
- **(A)** Add minimum geo upload requirements check.
- **(A)** Expand GEO Location information to cover manual upload.

#### Plugin(S) - Traffic Count
- **(B)** Fixed IP lock bug.

### Version 0.1.3 March 2013

#### Component - Traffic
- **(B)** Fixed geoip.inc conflicts.

#### Module - Traffic
- **(A)** Who is online display guests and members option.

### Version 0.1.2 February 2013

#### Component - Traffic
- **(A)** Geo location has been integrated into the system.
- **(A)** Install script integrated to allow all associated extensions to be installed at once.
- **(A)** New language strings added.
- **(C)** New columns added to the #__cwtraffic table to store country and city info.
- **(A)** Traffic Country and city statistics added to control panel.
- **(C)** Some settings have been moved to the component from the module to allow both the module and plugins access to them.
- **(A)** Known IP descriptions added to visitor layout. 

#### Module - Traffic
- **(C)** Some module options have been streamlined.
- **(A)** Who is online options added
- **(A)** New language strings added.
- **(C)** Some settings have been moved to the component from the module to allow both the module and plugins access to them.
- **(R)** Removed code to count visitors the system now uses a plugin.
- **(R)** Removed database cleanup code the system now uses a plugin.

#### Plugin(S) - Traffic Count
- **(N)** Integrated into the system

#### Plugin(S) - Traffic Clean
- **(N)** Integrated into the system

### Version 0.1.1 January 2013

#### Component - Traffic
- **(C)** New look and layout of the control panel.
- **(C)** Updated help system.
- **(A)** Option to export a CSV report of the visitors.
- **(A)** New language strings added.
- **(C)** Update language files.
- **(R)** Removed non English files they can now be download from CoalaWeb.com as needed.

#### Module - Traffic
- **(R)** Removed non English files they can now be download from CoalaWeb.com as needed.
- **(A)** Added unique module ID to reduce likely hood of conflicts. This will be expanded in future releases.
- **(R)** Removed several & symbols from helper file to avoid assignment by reference errors.

### Version 0.1.0 December 2012

#### Module - Traffic
- **(B)** Fixed JDatabase Query error.

### Version 0.0.9 November 2012

#### Component - Traffic
- **(C)** Language file tweaks.

#### Module - Traffic
- **(B)** Fixed php Notice due to undefined variable.
- **(C)** Language file tweaks.

### Version 0.0.8 November 2012

#### Component - Traffic
- **(A)** Added Italian translation.
- **(C)** Updated help file.
- **(C)** Language file tweaks.
- **(C)** Updated description images.
- **(B)** Fixed date and time calculation issue.

#### Module - Traffic
- **(A)** New arrows icon theme.
- **(A)** Added module help link.
- **(A)** Added Italian translation.
- **(A)** Added help link in module backend.
- **(R)** Removed time offset it is now based on Joomla server settings.
- **(R)** Removed date and time language options now they automatically changed based on Joomla language.
- **(C)** Update language strings.
- **(C)** Updated description images.
- **(C)** Redesigned the date and time display and store methods.
- **(C)** Expanded methods to identify IP. Now more reliable detection even behind a proxy.

### Version 0.0.7 September 2012

#### Component - Traffic
- **(C)** Language file tweaks.

#### Module - Traffic
- **(A)** New module configuration styling.
- **(C)** Update language strings.
- **(B)** Fixed preg match error in helper file.

### Version 0.0.6 August 2012

#### Component - Traffic
- **(A)** Visitor filter and search options added.
- **(C)** Update server location has moved.
- **(C)** Help file updated.
- **(A)** Added component search CSS.
- **(A)** New language string.

#### Module - Traffic
- **(A)** New icon style clocks added.
- **(C)** Update server location has moved.
- **(C)** Icon CSS tweaks.

### Version 0.0.5 July 2012

#### Component - Traffic
- **(A)** Added automatic database clean-up option

#### Module - Traffic
- **(A)** Added automatic database clean-up option

### Version 0.0.4 June 2012

#### Component - Traffic
- **(A)** Foundation for sql update allowing automatic database cleanup to be added to next release.
- **(L)** Added missing language string

#### Module - Traffic
- **(C)** Streamlined icons into sprites for faster loading.
- **(A)** Foundation for sql update allowing automatic database cleanup to be added to next release.

### Version 0.0.3 June 2012

#### Component - Traffic
- **(B)** Fixed non JURI::root referenced images.
- **(A)** Added Spanish (Spain) es-ES language
- **(A)** Added Portuguese (Brazil) pt-BR language

#### Module - Traffic
- **(C)** Set a default for getLayoutPath
- **(B)** Fixed non JURI::root referenced images.
- **(A)** Added new star theme for the module
- **(A)** Added Spanish (Spain) es-ES language
- **(A)** Added Portuguese (Brazil) pt-BR language

### Version 0.0.2 April 2012

#### Component - Traffic
- **(C)** Streamlined ACL code
- **(B)** Fixed description layout in Knownips form

#### Module - Traffic
- **(A)** Added new tag theme for the module
- **(B)** Fixed php Notice due to wrongly declared static function

### Version 0.0.1 March 2012

#### Component - Traffic
- **(N)** Initial release

#### Module - Traffic
- **(N)** Initial release

### Key
- **(S)** Security Fix
- **(B)** Bug Fix
- **(L)** Language fix or change
- **(A)** Addition
- **(C)** Change
- **(R)** Removed
- **(N)** Note