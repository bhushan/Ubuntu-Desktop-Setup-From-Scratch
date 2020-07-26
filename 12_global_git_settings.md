Set up git configuration:

run `touch ~/.gitignore` to create `.gitignore` file.

now add below lines:

```bash
echo ".idea" >> ~/.gitignore
echo ".vscode" >> ~/.gitignore
echo ".php_cs.cache" >> ~/.gitignore
```

`git config --global core.excludesfile '~/.gitignore'`
