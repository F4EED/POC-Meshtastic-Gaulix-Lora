# POC-Meshtastic-Gaulix-Lora
En parallèle du POC Gestion de Crise, voici la Brique Meshtastic/Gaulix/LoRa qui a l’image du projet présenté par la société Seeed Studio voici donc le POC que nous appellerons MPack pour Mission Pack.

Les rôles de celui sont :

    Géolocalisation des équipiers sur le terrain.
    Remontée d’informations depuis le terrain (télémétrie par exemple).
    échange de message court (sms) entre la base et les équipes sur le terrain.

Le tout en étant indépendant de tous réseaux commerciaux

Voici une petite description du MPack dans sa version actuelle :

Nous allons détailler tout cela :

- Noeud Meshtastic à base de Heltec V3 en 868MHz
- Système de BIP, alerte, réception message (doit être relié à un terminal Android ou iOS pour envoyer des messages)
- 2 systèmes de BIP, alerte, réception message (doit être relié à un terminal Android ou iOS pour envoyer des messages) à base de Heltec V3 868MHz
- Système de Bip tracker avec GPS intégré (doit être relié à un terminal Android ou iOS pour envoyer des messages) de chez Seeed Studio
- T-Deck, Un terminal complet et autonome (GPS, module LoRa, écran (couleur et tactile) clavier (qwerty)) de chez lilygo

- Une caisse de transport type « Pélicase ».
- Un clavier trackball en BT
- Un Raspberry pi 3
- Un écran tactile de chez Raspberry pi (c’est du luxe, mais j’avais ça sur de vieux projet).
- Des déports de port USB, Réseau.

Côté logiciels :

    - La distribution Linux d’origine Raspberry pi
    - Grafana
    - RabbitMQ
    - Node-Red

Suivant les applications à venir, d’autres arriverons surement;
Un réseau wifi

Pour relier le nœud Lora aux services du mapck, nous passons par un réseau Wifi qui s’appuie sur un router, GL Intet
Le point sur le projet

La partie Lora/meshtastic/Gaulix est en place et fonctionne correctement, les modifications à venir seront le boitier, l’autonomie et l’antenne.

Les logiciels installés sur le Raspberry pi sont tous fonctionnels, seules les parties RabbitMQ et noed-red sont utilisées pour le moment.

Voilà, au plaisir de vous retrouver pour la suite de la brique MPack

Frédéric

    PS pour tout ce qui concerne Meshtastic, Gaulix, retrouvez nous sur le site internet de Gaulix https://gaulix.fr/, vous trouverez sur le site internet tous les moyens possibles pour les contacter.
