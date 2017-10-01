Open
====
An Open Source Social Network. Available @ http://open.subinsb.com
Feel free to contribute and please report bugs if you find any.

If you need help, documentation and other info about Open, please see our blog : http://open.subinsb.com/blog

Note that the blog folder is not included in source code. The blog is ran using Wordpress.

The folder "cron" contains the CRON job files. Open the .php file in "cron" folder for more details.

Run On Localhost
====
Here is a simple tutorial on how to run Open on a Linux Apache Web Server.

1) Install Git by Running the following commands
```
sudo apt-get update && sudo apt-get install git
```

2) CD (Change Directory) to the Apache directory by running
```
cd /var/www/
```  
   in Apache Server versions 2.5 and above, the folder is `/var/www/html` instead of `/var/www`
      
3) Now do this to pull the source code from GitHub to the folder "open" in /var/www
```
git clone https://github.com/subins2000/open.git open
```
	Now open's files will be in the `/var/www/open` directory

4) 	Using Replacing Softwares like (http://regexxer.sourceforge.net/)[regexxer], replace the string `open.subinsb.com` with `localhost/open` on the directory where you cloned the open repository.
	Also, there might be URL strings like `open\.subinsb\.com` in certain files which won't be covered with this replacing. An example is `cdn/js/main.js` file on `open.externalLinks` function.

5) 	Create a MySQL database named "open"

6) 	Execute The SQL Code in the file [tables.sql](https://github.com/subins2000/open/blob/master/tables.sql)

8) 	Open file `config.php` of Open root directory and set the Database credentials.

9) 	Go To http://localhost/open to see Open live in action

Libraries used In Open
====
jQuery

The @Mentions have been implemented on Open by using [jQuery sMention Plugin](https://github.com/subins2000/smention)

[PHP OAuth Class](http://www.phpclasses.org/package/7700-PHP-Authorize-and-access-APIs-using-OAuth.html). Thanks Manuel Lemos.

Resize image class

Debug
=====
Pass "?show_errors=1" with the URL to see the errors, warnings omitted by PHP. Example : http://open.subinsb.com/?show_errors=1

License
=====

subins2000/open is licensed under the GNU General Public License v3.0

Permissions of this strong copyleft license are conditioned on making available complete source code of licensed works and modifications, which include larger works using a licensed work, under the same license. Copyright and license notices must be preserved. Contributors provide an express grant of patent rights.
