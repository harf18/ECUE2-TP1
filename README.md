# TP1 : GIT & GitHub Classroom

### Objectif

Se familiariser avec GIT / Github Classroom / Pull request

### Prérequis

- Ouvrir Git Bash, aller dans le dossier de votre choix et créer un dossier ECUE2. Par exemple :  

```
$ cd  
$ cd Documents  
$ mkdir ECUE2
$ cd ECUE2
```
- Sur github, sur la page d'accueil du projet, cliquer sur le bouton vert "code" et copier le l'url qui s'affiche (```https://github.com/Le-Cnam/tp1...```)
- Cloner le projet GITHUB sur votre poste :  

```
$ git clone <COLLER L'URL COPIEE CI DESSUS>  
```

- Saisir vos identifiants github  
- Git va récupérer le projet. Visualiser le dossier, puis aller dans le dossier :

```
$ ls -ltr
$ cd tp1-XXXXXX (ou XXXXX = votre username)
```

- Vous remarquez **(master)** en fin de ligne : vous êtes sur la branche master  

- Créer une nouvelle branche, puis aller sur la branche :  

```
$ git branch prenomNom
$ git checkout prenomNom
```

- Vous remarquez **(prenomNom)** en fin de ligne : vous êtes sur la branche prenomNom.  Git change le contenu de votre repertoire en fonction de la branche sur laquelle vous êtes. La branche master ne sera pas impactée par vos modifications.

  

### IntelliJ

- Ouvrez IntelliJ
- Ouvrir le projet ECUE2-TP1 :
	- Sur l'écran d'accueil d'IntelliJ, cliquer sur **Open**
	- Selectionner le dossier du projet et cliquer sur **OK**
	- Cliquer sur **File** puis **Project Structure...**
	- Dans **Language level** sélectionner **SDK Default**
	- Dans **SDK** sélectionner **add SDK** et selectionner votre jdk23
	- Sélectionner la version **23** et cliquer sur **Download**
	- Cliquer sur **Ok**

### Votre 1er programme Java 23

- Dans le navigateur de projet a gauche, developper **tp1-XXXXXX > src** en cliquant sur la fleche devant src
- Double cliquer sur HelloWorld : dans la fenêtre principale d'IntelliJ, la classe HelloWorld s'ouvre, ajouter le contenu nécessaire pour créer un Hello World.
- Pour l'excuter, cliquer droit sur **main** et cliquer sur "Run HelloWorld.main"
- Hello World doit s'écrire dans la fenêtre en bas d'IntelliJ



### Envoyez votre travail

- Dans GIT bash, ajouter votre travail dans la "zone prêt à commiter" :

```
$ git add .
```

- Commitez votre travail (faire un commit = enregister votre code dans l'historique des modifications) : 

```
$ git commit -m "<Un message de commit comprehensible et qui décrit bien votre travail>"
```

- Envoyer votre branch nomPrenom sur le serveur

```
$ git push origin prenomNom
```

- Aller sur GitHub et Cliquer sur **New Pull Request**, base = *master*, compare = votre branche *prenomNom*, puis cliquer sur **Create Pull Request**
