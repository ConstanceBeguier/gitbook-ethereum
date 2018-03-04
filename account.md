# Comptes (account)

Compte (account):
  - Etat: chaque compte possède un état contenant le solde pour un EOA et le solde et le contrat pour un contrat
  - Cyptosystème à clé publique: pour vérifier les identités des EOAs
  - Adresse d'un EOA: 20 derniers octets de sa clé publique
  - Keyfile: fichier texte JSON contenant la clé publique en clair et la clé privée chiffrée par un mot de passe
  - Création d'un compte EOA: 
```bash
geth  account new # or eth.accounts
```
  - Lister les comptes: 
```bash
geth  account list # or personal.newAccount()
```
  - Modifier le MDP:  
```bash
  geth  account  update [<uuid>|<address>,...]
```
  - Importer des clés: 
```bash
geth  account import [<uuid>|<file>|<secret-hex>]
```
  - Importer un porte-monnaie (wallet): 
 ```bash
 geth  wallet import <file>
 ```
  - Mist  Ethereum  wallet: interface graphique pour Ethereum

