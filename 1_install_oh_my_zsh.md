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
Go to terminal -> edit -> preferences  and change below settings 
In Text tab
- change cell spacing width to 1.50
- Terminal Bell untick 
In Colors tab
- untick Use colors from system theme

Now reboot system to changes to take efect.
