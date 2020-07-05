install required extensions
`sudo apt-get install php-curl libnss3-tools jq xsel`

get valet linux:

`composer global require cpriego/valet-linux`

now run `valet install` this will install nginx and will setup valet into machine.

Create a new directory on your machine by running something like `mkdir ~/Code`. Next,
`cd ~/Code` and run `valet park`.
This command will register your current working directory as a path that Valet should search for sites.

