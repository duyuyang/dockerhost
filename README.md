# dockerhost

## Build secure CentOS AMI for containers


## Build docker host on top of ubuntu

curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -

sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable edge"

apt-cache policy docker-ce

sudo apt-get install -y docker-ce

sudo systemctl status docker

sudo usermod -aG docker ${USER}

## Run applications in docker-compose
