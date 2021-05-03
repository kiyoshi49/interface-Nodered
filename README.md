# interface-Nodered

## Presentation du projet

Le but de ce projet est de mettre en place un systeme qui permet de mesurer l'affluence du fablab, d'avoir une meilleur vision de l'utilisation des machines, et aussi permettre un accès plus controllé aux machines

## Le choix technologique

Pour ce projet, nous partons d'une solution développée en Node-Red pour plusieurs raisons :
 - Node-red est installé par défault sur une distribution raspbian et donc on peut avoir le centre du système qui tourne sur un raspberry pi
 - Le bocal n'a pas des ressources énormes à consacrer à ce développement, le système node-red parrait une technologie rapide à prendre en main pour permettre aux membres du fablab de contribuer à ce developpement
 - il permet d'utiliser toutes les technologies qui devront permettre de mettre en place cette interface (SQlite pour la BDD, MQTT pour la communication entre modules, et une interface web simple)

## Architecture systeme

![node-red archi](https://user-images.githubusercontent.com/10775713/116858292-6f2a0600-abfe-11eb-9991-d13c4bf5d266.jpg)

## Fonctionnalitées

### Aujourd'hui 

Aujourd'hui on peut enregistrer via une interface web les interactions des membres dans le fablab, il faut à chaque fin d'utilisation des machines entrer le membre du fablab, les machines utilisées et son indépendance sur les machines.
Sur l'interface on peut ajouter un membre dans la base de données.

### Objectifs

L'information et la base de donnée doivent tourné sur le raspberry pi, plusieur module avec des esp32+RFID doivent permettre aux membres de badger
