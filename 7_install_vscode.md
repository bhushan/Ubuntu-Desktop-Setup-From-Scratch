import the Microsoft GPG key

`wget -q https://packages.microsoft.com/keys/microsoft.asc -O- | sudo apt-key add -`

enable the Visual Studio Code repository by typing:
`sudo add-apt-repository "deb [arch=amd64] https://packages.microsoft.com/repos/vscode stable main"`

now run 

```bash
sudo apt update
sudo apt install code
```
