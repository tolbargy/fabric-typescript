GUIAAAA ---> https://hyperledgerfabric-bg.github.io/guide


apt-get update
apt-get upgrade
sudo apt-get install build-essential gcc make perl dkms
iinstalra imagen vvirtuablox
instalar code
instalar chrome

-- INSTALAR CURL
sudo apt-get install cURL

-- INSTALAR DOCKER
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


-- INSTALAR DOCKER_COMPOSE
sudo curl -L "https://github.com/docker/compose/releases/download/1.27.4/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose

sudo chmod +x /usr/local/bin/docker-compose
sudo ln -s /usr/local/bin/docker-compose /usr/bin/docker-compose


-- INSTALAR GO

sudo apt-get install go-lang


-- INSTALAR NODEJS 8

sudo curl -sL https://deb.nodesource.com/setup_8.x | sudo -E bash -
sudo apt install nodejs


-- INSTALAR PYTHON 2.7

sudo apt-get install python2.7


-- CONFIGURAR IMAGENS Y TODO PARA BYFN (Building your first network in hiperledger fabric)

sudo curl -sSL http://bit.ly/2ysbOFE | sudo bash -s -- 1.4.6 1.4.6 0.4.18



-CLONAR https://github.com/hyperledger/fabric-samples 

- Pasarse a release-1.4 branch

- Ejecutar $ curl -sSL http://bit.ly/2ysbOFE | bash -s - 1.4.6 1.4.6 0.4.18

- Esto anterior para obtener los binarios en el subdirectorio actual y descargar todas las imagenes de hyperledger

- Agregamos el PATH a todo el sistema para poder acceder a los binarios

export PATH=/home/tolbar/Escritorio/workspace/red-blockchain/bin:$PATH

# Iniciar fabric javascript
cd fabcar && sudo ./startFabric.sh javascript