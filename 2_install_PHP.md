Run 

```bash
sudo apt -y install software-properties-common
sudo add-apt-repository ppa:ondrej/php
sudo apt-get update
```

Now install PHP 8.0 using `sudo apt -y install php`


verify running `php -v`

You may want to install in addition some extensions:

```bash
# Those extensions are often required
sudo apt install php-json php-curl php-mcrypt php-bcmath
```
