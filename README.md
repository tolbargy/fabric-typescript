# Basado en la guia de Hyperledger Fabric 1.4
https://hyperledgerfabric-bg.github.io

# Requisitos previos Ubuntu 18.04
apt-get update
apt-get upgrade
sudo apt-get install build-essential gcc make perl dkms

# Instalar curl
sudo apt-get install cURL

# Instalar Docker
sudo apt-get update
sudo apt-get install \
    apt-transport-https \
    ca-certificates \
    curl \
    gnupg-agent \
    software-properties-common
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
sudo apt-key fingerprint 0EBFCD88
sudo add-apt-repository \
   "deb [arch=amd64] https://download.docker.com/linux/ubuntu \
   $(lsb_release -cs) \
   stable"
sudo apt-get update
sudo apt-get install docker-ce docker-ce-cli containerd.io

# Instalar Docker Compose
sudo curl -L "https://github.com/docker/compose/releases/download/1.27.4/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
sudo chmod +x /usr/local/bin/docker-compose
sudo ln -s /usr/local/bin/docker-compose /usr/bin/docker-compose

# Instalar GO
sudo apt-get install go-lang

# Instalar NodeJS 8
sudo curl -sL https://deb.nodesource.com/setup_8.x | sudo -E bash -
sudo apt install nodejs

# Instalar Python 2.7
sudo apt-get install python2.7

# Instalar version antigua npm
sudo npm install npm@5.6.0 -g

# Instalar Node gyp y Node pre gyp
sudo npm install --global node-gyp
sudo npm install --global node-pre-gyp

# Ejecutar contrato
sudo ./startFabric.sh