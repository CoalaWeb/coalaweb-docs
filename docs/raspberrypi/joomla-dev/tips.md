Tips
Nano select and cut text
To select text in nano, move the cursor to the start of the text you want to select, press the Alt-A key combination to mark the start, then move the cursor to the end of the section you want to select.

press Ctrl+K to cut your selection and Ctrl+U to paste it.

More info can be found here: https://help.ubuntu.com/community/Nano

Nginx Logs
Nginx error logs can be found at the following location which are great for fault finding. The configuration used in this series will produce one per site making it easy to find and fix errors.

/var/log/nginx

Pi crash causing issues
Did you pi crash or loose connection while editing with Nano and now your sites aren’t working as expected? Check to see if the file below was automatically created as this could be overriding your conf files

nginx.conf.save 

If you remove it you should be back to normal

Raspberry Pi Configuration
If you ever need to get back to the Raspberry Pi configuration page use the following command.

sudo raspi-config 
