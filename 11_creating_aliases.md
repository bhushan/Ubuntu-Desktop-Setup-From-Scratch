```bash
touch ~/.aliases
```
copy following aliases to `.aliases` file.

```bash
alias cc="clear"
alias update="sudo apt update && sudo apt upgrade && sudo apt autoremove && sudo apt clean"
alias dump="composer dump-autoload -o"
alias watch="npm run watch"
alias wip="git add . && git commit -m 'wip'"
alias push="git push"
alias wpush="git add . && git commit -m 'wip' && git push"
alias nah="git reset --hard && git clean -df"
alias p="./vendor/bin/phpunit"
alias pf="./vendor/bin/phpunit --filter "
alias art="php artisan "
alias migrate="php artisan migrate"
alias fresh="php artisan migrate:fresh"
alias seed="php artisan migrate:fresh --seed"
```
now run `echo 'source ~/.aliases' >> ~/.zshrc`

and restart terminal to aliases to take effect.
