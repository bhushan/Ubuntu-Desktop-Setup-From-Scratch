Set up git configuration:

1) Global gitignore file.

run `touch ~/.gitignore` to create `.gitignore` file.

now add below lines:

```bash
echo ".idea" >> ~/.gitignore
echo ".vscode" >> ~/.gitignore
echo ".php_cs.cache" >> ~/.gitignore
```

`git config --global core.excludesfile '~/.gitignore'`

2) Global User Email/Name: 

Obviously email/name should be yours.

`git config --global user.email "bhushangaykawad@gmail.com"`

`git config --global user.name "Bhushan"`

3) Global Core Editor: 

`git config --global core.editor "vim"`

4) Git Credential Store:

`git config --global credential.helper cache`

