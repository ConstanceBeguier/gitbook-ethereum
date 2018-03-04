# Création d'une blockchain privée

Installation d'Ethereum:
```bash
sudo  apt-get  install software-properties-common
sudo add-apt-repository -y ppa:ethereum/ethereum
sudo  apt-get  update
sudo  apt-get  install  ethereum
```

Création du genesis block:
```bash
cd /home
mkdir private_blockchain
cd private_blockchain
# create genesis block into GenesisBlock.json
geth  init  genesis.json # start blockchain
geth  account new # create an account
geth --networkid 123 --nodiscover --maxpeers 0 console # launch console on this blockchain
```

