# FCSC 2020 Bluetooth Low Energy

Une personne de votre entourage ne jure que par le traitement du signal analogique. Pour lui montrer certains des avantages du traitement du signal numérique, vous décidez de le mettre au défi : il doit émettre des annonces Bluetooth Low Energy sur chacun des canaux d’annonce, tandis que vous ne disposez que d’une radio logicielle pour les capturer tous.

Vous lui montrez alors qu’en désactivant le filtre anti-repliement de l’étage d’entrée, vous arrivez à capturer toutes les communications.

La capture fournie ([ble.sig](ble.sig)) a été faite en désactivant le filtre anti-repliement, à la fréquence centrale 2461MHz et avec un taux d’échantillonnage de 20MHz.

Note 1 : Le format de fichier est une capture au format IQ, avec chaque échantillon I et Q un nombre flottant de 32 bits. Les logiciels de traitement du signal standard n’ont pas de problème à ingérer ce format. Note 2 : Pour ouvrir ce fichier avec numpy, il faut utiliser le format complex64 : numpy.fromfile(<filename>, dtype = numpy.complex64). Pour utiliser le logiciel GNURadio, il faut utiliser le bloc File Source et le format complex. Note 3 : Pour commencer à analyser la capture, vous pouvez utiliser le flowgraph fourni dans GNU Radio.


Les fichiers 
--------------
- [ble.sig](ble.sig)
- [gr_waterfall_tuto.png](gr_waterfall_tuto.png)





Auteur : ElyKar

Origine : [Bluetooth Low Energy](https://hackropole.fr/fr/challenges/hardware/fcsc2020-hardware-bluetooth-low-energy/)



-----------

## Installation manuel
Vous n'utilisez pas l'application **les CTFs de Cyrhades** ? C'est dommage !
Mais voici comment installer ce CTF manuellement :

> git clone https://github.com/Hack-Oeil/fcsc2020-hardware-bluetooth-low-energy.git

> cd fcsc2020-hardware-bluetooth-low-energy


-----------

## Sur le site officiel hackropole.fr
> https://hackropole.fr/fr/challenges/hardware/fcsc2020-hardware-bluetooth-low-energy/


