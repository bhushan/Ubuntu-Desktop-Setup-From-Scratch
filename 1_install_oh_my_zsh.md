* Install zsh `sudo apt install zsh`

* Install GIT `sudo apt install git` and confirm running `git --version`

* Install Oh my zsh

`sh -c "$(wget https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh -O -)"`

TIP: to set zsh as default run `sudo chsh -s $(which zsh) $(whoami)`

* Install Powerline font `sudo apt install fonts-powerline`

* Install VIM `sudo apt install vim`

now run `sudo vim ~/.zshrc` and change ZSH_THEME variable to ZSH_THEME="agnoster".

To remove the username and host from the prompt, modify:

`sudo vim ~/.oh-my-zsh/themes/agnoster.zsh-theme`
```
## Main prompt
build_prompt() {
  RETVAL=$?
  prompt_status
  prompt_virtualenv
  prompt_aws
  #prompt_context
  prompt_dir
  prompt_git
  prompt_bzr
  prompt_hg
  prompt_end
}
```

Now reboot System to see changes
