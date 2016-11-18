In the old days to check your PHP setting you would have used a PHP function called phpinfo() or manually looked at the contents of your server files but in modern Joomla installations you can use the **System Information** section.

So lets start by logging into the Admin area of your Joomla website and from the top menu go to:

image

In the next window we have two PHP related tabs **PHP Settings** and **PHP Information** for this guide we are interested in the information tab

Now the first bit of information we are interested in is where are your setting coming from. Many of us tend to open a php.ini file located somewhere on our website and looking up the parameter setting. This is not an accurate way of determining the actual value that your Joomla environment is experiencing. Use the Joomla backend for this.

Another nice bit of data you can pick-up from the “PHP Information” tab is to search for ‘Loaded Configuration File ‘. The line that will appear in your browser will show you exactly which php.ini file your environment is loading.

let have a look at the importa setting that will affect uploads:

-   file_uploads

file_uploads determines whether uploads can be made to the server via HTTP or not. If this is set to OFF, no uploads of any kind are allowed.

-   upload_max_filesize

upload_max_filesize limits the maximum size of an individual file be uploaded. Normally, this value is entered in MB (Megabyte). During FTP upload this value concerns the size of each individual file. During batch upload, however, this value concerns the size of the entire zip file you upload, which is where limitations can make themselves more easily apparent.

-   post_max_size

upload_max_filesize is not the only value that determines the maximum size of a file to be uploaded. post_max_size is among the settings that influence upload_max_filesize. It determines the maximum size of POST files. Usually, file uploads are POST files. To allow the upload of larger files, the value given in post_max_size must be larger than the value in upload_max_filesize.

memory_limit

memory_limit determines the maximum amount of memory that a script may take up during an operation. The value is usually given in bytes. This value should be larger than the one given in post_max_size. A value of -1 means that there are no limitatons. As the exact amount of memory used by a script during upload is difficult to predict, memory_limit is a setting to watch out for.The above three settings are essential in configuring file uploads.

memory_limit >> post_max_size > upload_max_filesize

If upload_max_filesize was set to 2 MB, a batch upload of 4MB zip file for example would simply be bound to fail.

These 3 settings, however, are not the only ones that determine a smooth functioning of your file uploads. Another important setting, well capable of ruining your uploads even if correct values were set for upload_max_files, post_max_size and memory_limit, is this:

    max_execution_time

max_execution_time defines the maximum time (in seconds, or rather miliseconds!) that a script is allowed to take up in order to perform an operation. If it takes any longer, the parser (=server side software that interpretates the script in accordance to the current settings) will halt the execution. This is a critical matter especially for uploads, as upload and extraction of a large zipfile, image copying and resizing etc. all take their time. 

How to change it?
On your localhost environment, you can basically edit this php.ini file using your text editor, search for the relevant parameter lines, update them and save changes. You will most likely need to restart your webserver (or even reboot).

On a remote hosting environment, if you do not have access to this file you will need to contact your host helpdesk and have them make any changes needed for you to increase the ‘upload_max_filesize’ php parameter. Actually, even if you do have access and can modify it, better be safe and open a ticket with your helpdesk as additional steps might be needed from their end (e.g., perhaps server restart is needed depending on hosting package).

If your host helpdesk refuses, you should seriously consider looking for a new host. This is a simple setting and there is really no real argument for not having this set to at least 8M.