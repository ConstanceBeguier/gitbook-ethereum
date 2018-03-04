# Réseau

  - EthStats.net et EtherNodes.com: dashboards de statistiques sur Ethereum
  - Public blockchain: blockchain ouverte à tous pour l'envoi de transactions et le minage
  - Consortium blockchain: par exemple, un consortium de 15 institutions financières et au moins 10 doivent signer un bloc pour qu'il soit validé
  - Private  blockchain: écriture restreinte à une organisation, lecture restreinte ou non
  - Nb de noeuds auxquels on est connecté: 
```bash
net.peerCount
```
  - Info sur les noeuds voisins: 
```bash
admin.peers
```
  - Importer/exporter la blockchain: 
```bash
geth import/export <filename>
```
 - Static node: noeud auquel on veut toujours rester connecté
 - Uniquement des noeuds statiques: 
```bash
--nodiscover
```
  - Réseau de test: nom Modern 
```bash
--modern
```

Réseau local de test
  - Fichier genesis: 
```bash
--genesis  CustomGenesis.json
```
```bash
{ "nonce": "0x0000000000000042", "timestamp": "0x0",
"parentHash":  "0x0000000000000000000000000000000000000000000000000000000000000000", 
"extraData": "0x0", "gasLimit": "0x8000000", "difficulty": "0x400", 
"mixhash": "0x0000000000000000000000000000000000000000000000000000000000000000",
"coinbase": "0x3333333333333333333333333333333333333333", "alloc": { }} 
```
  - Dossier de données: 
```bash
--datadir "/home/TestChain1"
```
  - ID du réseau: 42
  - Désactiver la recherche de noeud: 
```bash 
--nodiscover
```
  - Nombre de noeuds maximum: 
```bash 
--maxpeers <nb>
```
  - Remote  Procedure  Call  RPC: 
```bash
--rpc --rpcapi "db,eth,net,web3"
--rpcport "8080" --rpccorsdomain <"url">
```
  - Network  listening port: 
```bash
--port "30303"
```
  - Identité du noeud: 
```bash 
--identity "TestnetMainNode"
```
  - Lancer le nouveau réseau
```bash
geth --identity "MyNodeName" --rpc --rpcport "8080" --rpccorsdomain
<url> --datadir <dir>
```
 - Allouer de l'argent lors de la création de la blockchain: ajouter dans le fichier CustomGenesis.json
```bash
"alloc": { "<account_address>":  { "balance": "200" } }
```

