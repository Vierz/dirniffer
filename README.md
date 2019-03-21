# About
Dirniffer is a simple tool to list all the hidden directories of a website using a wordlist and also it checks if the robots.txt is present and list all the disallowed directories.

# Setup
- **Download:** [dirniffer](dirniffer)
- **Make it executable:** chmod +x dirniffer
- **Move the file to:** /usr/sbin

# Use
- **Run the command as follows:**  dirniffer url wordlist.txt
- **NOTE:** for https URLs please always use https:// when running the command
- **Example:** 
```console
vierz@hostname:~$ dirniffer https://domain.com directorywordlist.txt 

Disallowed directories in robots.txt

/CHANGELOG.txt
/cron.php
/INSTALL.mysql.txt
/INSTALL.pgsql.txt
/INSTALL.sqlite.txt
/install.php
/INSTALL.txt
/LICENSE.txt
/MAINTAINERS.txt
/update.php
/UPGRADE.txt
/xmlrpc.php
/admin/
/filter/tips/
/node/add/
/search/
/user/register/
/user/password/
/user/login/
/user/logout/
/?q=admin/
/?q=filter/tips/
/?q=node/add/
/?q=search/
/?q=user/password/
/?q=user/register/
/?q=user/login/
/?q=user/logout/

Found directories using directorywordlist.txt

/includes/
/misc/
/modules/
/profiles/
/scripts/
/themes/

```
