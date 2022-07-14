# Wordpress-Installation
No apache 2.0 or httpd required to be installed. PHP is the main source to use to be able to run wordpress and any other site that uses php documents without configuring apache. Since PHP is depreciated, this is recommended.
<br>

### Packages
- [ ] PHP (latest version)
- [ ] MYSQL (Latest Version) -> Download from webpage
- [ ] WGET (Download wget)
- [ ] Homebrew -> Watch official site


#### Steps
- [ ] Install homebrew with the following script: `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"` to install in mac, use official sites for other os
- [ ] Install PHP on the official site: [PHP8.0](https://www.php.net/)
- [ ] Follow the steps to add php to path, recommended to use `micro` editor for easier use.
- [ ] *Edit* the  `/opt/homebrew/etc/php/version/php.ini`. which sets the maximum file site for php
```php
upload_max_filesize = 10M
``` 
- [ ] Install `mysql` (latest version) on mac.
- [ ] run `mysql -u root -p`, and submit the admin password.
- [ ] inside `mysql shell` run th following:
	- `CREATE DATABASE wordpress;` to create the main database
	- `\q or exit` to exit mysql
- [ ] <mark>Create a folder</mark> `mkdir /development/<your site name>` in the downloads folder (optional)
you can make the folder in an exxternal drive.
- [ ] *cd* into the folder and install wget in your os 
- [ ] `wget` the link to download the latest download version
	- `wget http://wordpress.org/latest.tar.gz`
	- `tar xfz latest.tar.gz`
	- `mv wordpress/* ./`
- [ ] Finally run a php server inside the folder with the following command: `php -S localhost:8000`
	- Port can be changed.
- [ ] follow the site steps to configure Wordpress for development.


##### Conclusion
**Subscribe & Like**
Youtube Channel: SimpleGameTutorials
Tutorial Site: [Follow the Creator](https://rkakodker.medium.com/how-to-setup-wordpress-in-m1-mac-local-cli-34104a680a2e)



**Star the project to reach to 300k to learn how to develop a personal blog an post it into the web free.**


