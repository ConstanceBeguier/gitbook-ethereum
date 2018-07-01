# Contrats et transactions

**Externally  owned  accounts (EOAs)**
  - possède un solde
  - peut envoyer des transactions
  - est controllé par une paire de clés privées
  - n'a pas de contrat associé

**Contract  accounts:**
  - possède un solde et un code/contrat
  - le code a son propre stockage et peut appeler d'autres contrats

**Transaction:** message entre deux comptes sur la blockchain
  - contient une signature identifiant l'envoyeur
  - le montant en wei du transfert
  - un contrat (optionel)
  - STARTGAS: nombre maximum de calculs pour l'exécution de cette transaction
  - GASPRICE: frais maximum que l'envoyeur est prêt à payer

**Contrat:** code (en Solidity compilé pour pouvoir être exécuté par l'EVM) et états (données) stockés à une adresse spécifique dans la blockchain
  - Liste des compilateurs disponibles: 
```bash
web3.eth.getCompilers();
```
  - Compiler contrat: 
```bash
contract = eth.compile.solidity(<file>)
```
  - IDE: Mix

