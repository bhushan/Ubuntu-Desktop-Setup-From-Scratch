give permissions to current user 
`sudo chown -R $USER ~/.composer` 

install required extensions 
`sudo apt -y install php7.4-zip php7.4-mbstring php7.4-xml`

now run

```bash
echo 'export PATH="$PATH:$HOME/.composer/vendor/bin"' >> ~/.zshrc 
composer global require laravel/installer
cd ~ && mkdir Code && cd Code
```

now create test project 

`laravel new test`
