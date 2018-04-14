# Upgrade local XAMPP installation

The current situation is that XAMPP already have been installed yet on the local maschine.
Instead of installing the new version on top of the current one, decided to choose the better variant and make a clean new installation.

### Guide

1. Stop all running services such as your `Apache` and `MySQL` server, then quit `XAMPP`.

2. Finally, rename the folder that `XAMPP` is installed in, for example, to **`xampp.OLD`**.

3. Then, install new `XAMPP` version like the first time.

4. Now, you have to make sure the new installation behaves just like the old one.

##### Move your data

5. Move your local *host-files* from the source-folder to the new destination-folder. You can find the files in `htdocs/`.

6. Move your local *databases* from the source-folder to the new destination-folder. You can find the databases in `mysql/data/`.

##### Merge customization of the different configuration files

| Module | Path to config file |
| ------ | ------ |
| XAMPP | `xampp-control.ini` |
| Apache | `apache/conf/extra/httpd-vhosts.conf` |
| PHP | `php/php.ini` and move your relevant extensions from extentions `php/ext/` |
| MySQL | `mysql/bin/my.ini` |
| phpMyAdmin | `phpMyAdmin/config.inc.php` |