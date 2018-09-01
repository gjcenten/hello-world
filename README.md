# hello-world
Test repository to get familiar with git commands and branches

NOTE: follow these steps to use the repo from the Linux shell
1) do a git clone

git clone https://github.com/gjcenten/hello-world.git

2) add the ~/.ssh/id_rsa.pub key to the project

3) Change .git/config:

Default:
[remote "origin"]
        fetch = +refs/heads/*:refs/remotes/origin/*
        url = https://github.com/gjcenten/hello-world.git

Should be:
[remote "origin"]
        fetch = +refs/heads/*:refs/remotes/origin/*
        url = ssh://git@github.com/gjcenten/hello-world.git

This doesn't work behind a proxy from a VBox VM !

01-09-2018:
Added pub ssh key for oberon
