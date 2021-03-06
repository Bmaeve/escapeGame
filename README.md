Projet WEB « Escape game » géographique 
=======
Département Informatique de l'ENSG - Géomatique   
Programmation WEB avancée

## Table des matières
1. [Informations](#Informations)
2. [Pré-requis](#Pré-requis)
3. [MAMP](#MAMP)
4. [WAMP](#WAMP)
5. [Consignes](#Consignes)
6. [Source](####Sources)

# Informations
#### Auteurs
Ilona Baran et Maeve Blarel
#### Date
1/11/2021 au 28/11/2021 (4 semaines)
#### URL du site
http://localhost/projetweb/pagePrincipale.php
#### Le Projet et ses objectifs:
L’objectif de ce TP est de créer un « escape game », notamment en résolvant des énigmes et en trouvant 
des objets. Le tout, sur une carte web.
Nous avons réalisé un « escape game » qui s'intitule: Tour de promo.
#### Langages utilisés
+ HTML5, CSS3
+ JavaScript, AJAX
+ PHP, MySQL
#### Responsive ?
Oui, il est responsive.

***

# Pré-requis
+ Installation de MAMP ou de WAMP  
+ Connection internet pour l'affichage de la carte  
+ Utilisation d'un navigateur (évitez Microsoft Edge et Internet explorer)

***

# MAMP

#### Récupération du projet #
Aller sur https://github.com/IlonaBaran/projetweb.git et télécharger le ZIP du projet 

![PojetWeb](images/readme/telechargementProjet.png)   
// après je ne sais pas ou il faut le placer :((

### Import de la base de données #
Ouvrir Mamp. 
Aller dans MAMP/Préférences/Web server et vérifier que le "document root" est bien l'emplcament où se trouve le projet récupéré. Dans le cas contraire, déplacer le projet dans le dossier explicité par le document root ou changer le document root (cela risque d'être plus compliqué).  
Dans un navigateur, aller sur http://localhost/phpmyadmin.  
Créer une base de données « escape game ».  
Importer le fichier espacegame.sql à cet emplacement.  
Ouvrir dans un éditeur de texte le fichier connexion.php, et modifier, au besoin, de telle façon à avoir ce qui suit : $link = mysqli_connect('localhost','nom','nom', 'escapegame');   
Penser à remplacer nom par votre prénom. // EST ce que c'est utile de dire ca ?    
![PojetWeb](images/readme/connexionBDDMAMP.png)  

Créer un compte d'utilisateur dans http://localhost/phpmyadmin en suivant les instructions suivantes:
![PojetWeb](images/readme/ajouterCompteBDD.png)

![PojetWeb](images/readme/creationCompteBDD.png)

puis "éxécuter" en bas de la page.  
Bravo, vous allez bientôt pouvoir commencer à jouer !

***

# WAMP 

#### Récupération du projet #
Aller sur https://github.com/IlonaBaran/projetweb.git et télécharger le ZIP du projet 
![PojetWeb](images/readme/telechargementProjet.png)
Extraire le projet et le mettre dans .../wamp64/www

### Import de la base de données #
Ouvrir WAMP. 
Aller dans MAMP/Préférences/Web server et vérifier que le "document root" est bien l'emplcament où se trouve le projet récupéré. Dans le cas contraire, déplacer le projet dans le dossier explicité par le document root ou changer le document root (cela risque d'être plus compliqué).  

Dans un navigateur, aller sur http://localhost/phpmyadmin.  
Se connecter sans changer l'identifiant et le mot de passe pré-rentré. Normalement, vous devriez avoir :   
![PojetWeb](images/readme/phpmyadminAccueil.png)

Créer une base de données « escape game ».   
Importer le fichier espacegame.sql à cet emplacement.   
Ouvrir dans un éditeur de texte le fichier connexion.php, et modifier, au besoin, de telle façon à avoir ce qui suit : $link = mysqli_connect('localhost','root','', 'escapegame');   
![PojetWeb](images/readme/connexionBDDWAMP.png)

Bravo, vous allez bientôt pouvoir commencer à jouer !

***

# Consignes
Le jeu comporte 3 pages :   
- une page principale.   
Vous devrez rentrer un pseudo pour pouvoir commencer à jouer. Celui-ci doit faire entre 1 et 20 caractères.   

- une page de jeu   
Pour pouvoir jouer au jeu, vous devez :   

+ Lorsque vous voyez le bouton "Suivant", vous devez cliquer dessus   
+ Vous devez validez la saisie d'un champ texte en appuyant sur la touche entrée

- une page de fin   
Vous pourrez voir le temps que vous avez mis à réaliser le jeu ainsi que votre position par rapport aux autres joueurs.  
Le retour à la page principale est permis grâce à un bouton. 


### Cahier de bord : Organisation au jour le jour // ca j'aurai pensé l'enlever, je ne sais pas quoi mettre dedans 

### Difficultés et solutions techniques rencontrées // idem, je ne sais pas trop quoi mettre si ce n'est parlé des fetch ou jsp

# Sources
La fonction strNoAccent de la page carte.js
