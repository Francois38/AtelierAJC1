# CAPTURE 2

## 1/ Pouvez vous interpréter la commande dig @ns1.google.com ...............

La commande dig permet de diagnostiquer les résolutions de noms DNS
Test de résolution de noms distante car @
TXT : le type 'Text string' de réponse attendu par le client
+short: pour avoir seulement l'adresse IP sans les autres informations

**On obtient en retour l'adresse IP de myaddr.l.google.com tel qu'indiqué dans le serveur DNS dns1.google.comde google**

## 2/ Capturez le trafic de cette commande

cf capture2.pcapng

## 3/ Combien de transactions sont-elles générées ? Pourquoi y en a-t-il autant ?

**2 transactions**, **une requête** envoyé par le client au serveur DNS directement et **la réponse du serveur DNS**

Le 1er serveur DNS avait directement l'information dans sa table de routage

## 4/ Pour chacune des transactions quelle est la question (QUERY) qui est posée ?

**Transaction 1 : o-o.myaddr.l.google.com**

**Transaction 2 : idem**


## 5/ Pour chacune des transactions a quel ordinateur est posée la question ?

**Transaction 1 : le PC1 ubuntu d'adresse IPv4 192.168.1.1**

**Transaction 2 : le serveur DNS de google 216.239.32.10**
