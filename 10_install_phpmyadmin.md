download phpMyAdmin latest zip from https://www.phpmyadmin.net/downloads/


extract it to `~/Code/phpmyadmin` rename if required folder to easy access via valet.

copy config file using `cp config.sample.inc.php config.inc.php`

open `config.inc.php` and edit it as below

```php
/* Authentication type */
$cfg['Servers'][$i]['auth_type'] = 'config';
/* Server parameters */
$cfg['Servers'][$i]['host'] = 'localhost';
$cfg['Servers'][$i]['compress'] = false;
$cfg['Servers'][$i]['AllowNoPassword'] = true;
$cfg['Servers'][$i]['username'] = 'root';
$cfg['Servers'][$i]['password'] = '';
```

now got to `phpmyadmin.test`.



