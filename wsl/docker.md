# Install and run docker on WSL ubuntu
How to install docker on WSL ubuntu distro?
1. wsl --update
2. wsl --list --online
3. wsl --install Ubuntu-22.04
4. sudo apt update -y
5. sudo apt install docker.io -y
6. sudo service docker start
7. sudo usermod -aG docker ${USER}
8. mkdir -p ~/.docker
9. touch ~/.docker/config.json
10. sudo chown $USER:$USER ~/.docker/config.json
11. vi ~/.docker/config.json

```
{
        "auths": {
        },
        "credsStore": "wincred"
}
```
