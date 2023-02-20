# Docketu Micro Service

Projet de démonstration pour la mise en place d'un micro service sur le serveur Docketu de l'Université de Lorraine.

- Créer un fichier .env à la racine, basé sur .env.model

- Dans `./docker-compose.yml` :
    - remplacer le port externe (3333) par le port alloué par Docketu (de 1024 à 65000). Dans cet exemple, le port __64999__ est utilisé.
    - indiquer `version: '3'` 

- Installation des dépendances NPM dans le service Docker Node.js :

    `docker-compose run --rm nodejs npm install`

- Démarrage des services :
    `docker-compose up -d`

- Consultation du service :

    `curl -i http(s)://docketu.iutnc.univ-lorraine.fr:{port}`

    `curl -i http(s)://docketu.iutnc.univ-lorraine.fr:64999`

- Informations complémentaires dans ./docketu.pdf

--

<img src="https://sherpa.one/images/sherpa-logotype.png" width="120px">

__Alexandre Leroux__

_Enseignant / Formateur_<br>
_Développeur logiciel web & mobile_

Nancy (Grand Est, France)

https://sherpa.one
