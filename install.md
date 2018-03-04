# Installation

Installation avec docker:
```bash
docker pull ethereum/client-cpp
mkdir -p ~/.ethereum ~/.web3
docker run --rm -it -p 127.0.0.1:8545:8545 \
-p 0.0.0.0:30303:30303 -v ~/.ethereum:/.ethereum \
-v ~/.web3:/.web3 -e HOME=/ \
--user $(id -u):$(id -g) ethereum/client-cpp \
docker-eth
```

Installation Ubuntu:
```bash
sudo  apt-get  install software-properties-common
sudo add-apt-repository -y ppa:ethereum/ethereum
sudo  apt-get  update
sudo  apt-get  install  ethereum
```
  
Liens pour le client go-ethereum:
  - Wiki: https://github.com/ethereum/go-ethereum/wiki/geth
  - Website: http://ethereum.github.io/go-ethereum/
  - GitHub: https://github.com/ethereum/go-ethereum

