# INSTALLING DOCKER ON UBUNTU

`sudo apt update`

`sudo apt install apt-transport-https ca-certificates curl software-properties-common`

`echo \
  "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.asc] https://download.docker.com/linux/ubuntu \
  $(. /etc/os-release && echo "$VERSION_CODENAME") stable" | \
  sudo tee /etc/apt/sources.list.d/docker.list > /dev/null`

`sudo apt-get update`

Verifying the installation...

`sudo docker run hello-world`
