# Pipelie Gitlab avec une application NodeJS
Ce projet a pour objectif de tester concretement l'exécution du pipeline proposé par GitLab. 

## Déroulé
Le pipeline contient les jobs permettant de réaliser les tâches suivantes : 
- tests
- buid Docker image
- push Docker image to GitLab registry
- Deploy 

## Exécution en local
Prérequis : NodeJS (en version 18)
Ce projet peut être exécuté sur une machine locale avec les commandes suivantes : 
Installations des dépendances : 
    ```
    npm install
    ```

Lancement de l'application 
    npm run start

Exécution des tests 
    npm run test 

## Exécution avec Docker
Prérequis : Docker
Ce projet peut être exécuté sur une machine locale avec les commandes suivantes :
Build de l'image Docker
    `docker build -t node-app .`

Run de l'image Docker
    `docker run -d -p 3000:3000 node-app`