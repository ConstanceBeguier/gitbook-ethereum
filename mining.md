# Minage

  - Travail des mineurs: proof of  work (ethash) jusque mi 2017 et proof of  stake après mi 2017
  - Block time: 15 secondes entre deux blocs en moyenne
  - Récompenses: proportionnelles à la hashrate du mineur (nombre de nonces testés par seconde divisé par le hashrate total du réseau)
  - Commencer à miner: 
```bash
geth --mine --minerthreads=4
# or with the console
miner.start(4)
miner.stop()
```
  - Compte pour le minage: 
```bash
miner.setEtherbase(eth.accounts[2])
```
  - Afficher son hashrate: 
```bash
miner.hashrate
```

