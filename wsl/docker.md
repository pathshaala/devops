# Install and run docker on WSL ubuntu
How to install docker on WSL ubuntu distro?
1. wsl --update
2. wsl --set-default-version 2
3. wsl --list --online
4. wsl --install Ubuntu-22.04
5. sudo apt update -y
6. sudo apt install docker.io -y
7. sudo service docker start
8. sudo usermod -aG docker ${USER}
9. mkdir -p ~/.docker
10. touch ~/.docker/config.json
11. sudo chown $USER:$USER ~/.docker/config.json
12. vi ~/.docker/config.json

```
{
        "auths": {
        },
        "credsStore": "wincred"
}
```
