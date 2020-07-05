give permissions to current user 
`sudo chown -R $USER ~/.composer` 

install required extensions 
`sudo apt -y install php7.4-zip php7.4-mbstring php7.4-xml`

now run

```bash
composer global require laravel/installer
cd ~ && mkdir Code && cd Code
```
