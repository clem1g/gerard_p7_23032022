# GROUPOMANIA
En tant que nouveau developpeur de la société, je dois mettre en place un reseau social interne de manière à permettre une meilleure cohésion au sein du groupe Groupomania.
Il m'a été donné carte blanche pour mettre en place le back-end et le front-end avec pour objectif de develloper une application proche de Reddit ou 9GAG.

## Contexte : 
Voici les exigences du comité de direction :
- la présentation des fonctionnalités doit être simple ; 
- la création d’un compte doit être simple et possible depuis un téléphone mobile ;
- le profil doit contenir très peu d’informations pour que sa complétion soit rapide ;
- la suppression du compte doit être possible ; 
- l’accès à un forum où les salariés publient des contenus multimédias doit être présent ;
- L’accès à un forum où les salariés publient des textes doit être présent ; les utilisateurs doivent pouvoir facilement repérer les dernières participations des employés ; 
- le ou la chargé-e de communication Groupomania doit pouvoir modérer les interactions entre le ou la chargé-e de communication Groupomania doit pouvoir afficher les dernières participations des employés salariés
- La base de données doit se manipuler avec le language SQL
- Les données de connexion doivent être sécurisées
- Le projet doit être inclusif en respectant les standards du WACG 


## Reflexions fonctionnelles sur la partie User & Modération

1. Utilisateur “lambda” doit pouvoir :
    - créer un compte avec : nom - prénom - email - mot de passe 
    - Se logger à partir de son email & mot de passe
    - L’utilisateur doit pouvoir poster un texte et/ou une image ou un lien
    - L’utilisateur doit pouvoir modifier ou supprimer son post 
    - L’utilisateur doit pouvoir voir les posts des autres utilisateurs et retrouver simplement un post :
            Faire apparaitre les posts du plus récent au plus anciens
    - L’utilisateur doit pouvoir commenter un post

2. Le modérateur doit pouvoir : 
    - créer un post 
    - supprimer un post 
    - supprimer un commentaire 
    - Commenter un post 



## Technologies, logiciels,langages,frameworks, plugins utilisés
- Visual Studio Code
- Git, GitHubDesktop & Github
- Html, CSS , JS

- Backend :
    a. NodeJs
    b. Nodemon
    c. Sequelize
    d. Express
    d. Bcrypt
    g. JsonwebToken
    i. Multer

- Frontend
    a.Vuejs - Vuex
    b.Axios
    d.Boostrap Vue

## Pour lancer le projet

- Il faut créer un dossier "images" dans le dossier backend

 Installez nodes et les dépendances de chaque dossier 
- cd frontend puis npm i
- cd backend puis npm i 


Ensuite lancer l'excution de chaque dossier :

- cd frontend && npm run serve

- cd backend && nodemon server

==> http://localhost:8000/

La base de données etant en local dans le cadre de ce MVP, les fichiers de migrations et de models sont dans le repertoire. Il vous suffira des les importer dans votre ORM SQL
Il faut pour cela executer  : 
- npx sequelize-cli db:migrate

Pour plus d'information concernant la création de la base de données : https://sequelize.org/docs/v6/other-topics/migrations/
