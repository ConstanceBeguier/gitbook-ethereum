# Ether et Gas

## Ether  denominations:

  - $$10^3$$  wei = 1 Kwei (babbage)
  - $$10^6$$ wei = 1 Mwei (lovelace)
  - $$10^9$$  wei = 1 Gwei (shannon)
  - $$10^12$$  wei = 1 microether (szabo)
  - $$10^15$$  wei = 1 milliether (finney)
  - $$10^18$$  wei = 1 ether

Envoyer des ethers à partir de la console geth:
```bash
var sender = eth.accounts[0];
var receiver = eth.accounts[1];
var amount = web3.toWei(0.01, "ether")
eth.sendTransaction({from:sender, to:receiver, value: amount})
```

## Gas

  - Gas: coût estimé d'une transaction (si la valeur de l'ether augmente, le prix du gas doit diminuer et inversement)
  - Gas  Cost: cout statique d'un calcul en gas
  - Gas  Price: prix de change entre gas et ether
  - Gas  Limit: maximum valeur de gas par bloc 
  - Gas  Fee: frais de transaction en gas payé au mineur

