# Solidity

Installation:
```bash
git clone --recursive  https://github.com/ethereum/solidity.git
cd solidity
./scripts/install_deps.sh
mkdir  build
cd build
cmake .. &&  make
```

Structure d'un contrat:
  - Variable d'état (stockée dans le contrat): 
```bash
uint data
```
  - Fonctions: partie exécutable d'un contrat: 
```bash
function <name>(<param_types>) [internal|external] [constant] [payable] [returns (<return types>)] {...}
```

Par défaut une fonction est internal
  - Modifiers: modifier le champ d'une fonction:
```bash 
modifier onlyBefore(uint t) { if (now >= t) throw; _;  }
function bid() onlyBefore(time) {...}
```
  - Events: utiliser les log services de l'EVM: 
```bash
event  AuctionEnded(address  winner, uint  amount);
```
  - Structs: regroupement de plusieurs variables
```bash
struct Voter { uint  weight; bool voted; uint vote; }
```
  - Enums: type de données avec un nombre fini de valeurs possibles
```bash
enum  State  { Created, Locked, Inactive }
```

