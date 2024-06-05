# Billapp

## Comment lancer l'API en local:

Il faudra au préalable créer un repertoire bill-app. Les commandes qui vont suivre peuvent être executer via le terminal de VS Code.

### Cloner le projet:
```
git clone https://github.com/OpenClassrooms-Student-Center/Billed-app-FR-Back.git
```

### Utilisez une version de node compatible
Si vous utilisez une version récente de node sur votre ordinateur, il se peut qu'il y ai des erreurs lors de l'installation de certaines dépendances. Pour cela il est important de vous assurer que vous ayez une version de node compatible par exemple node v16 ou v18. 

Voici quelques indications pour gérer les version de node sur votre ordinateur: 

#### Sur Windows
- Installer NVM pour windows (https://github.com/coreybutler/nvm-windows/tags)
- changer la version de node pour une version compatible (par exemple 18.16.1) pous cela suivre les instruction de NVM pour windows : 
    - `nvm install 18.16.1`
    - `nvm use 18.16.1`
- Ouvrir Powershell en mode administrateur
- Entrer la commande «  Set-ExecutionPolicy RemoteSigned » pour pouvoir gérer l’execution de scripts dans powershell
- Fermer toutes les instances de terminal
- entrer la commande `npm install -g win-node-env` pour installer la gestion des variables d’environnement node pour window

### Clonez le projet frontend dans le dossier bill-app :
```
git clone https://github.com/OpenClassrooms-Student-Center/Billed-app-FR-Front.git
```

### Voici ce que vous devez obtenir :
bill-app/
   - Billed-app-FR-Back
   - Billed-app-FR-Front

### Acceder au repertoire du projet backend :
```
cd Billed-app-FR-Back
```

### Installer les dépendances du projet backend :
```
npm install
```

### Lancer l'API :
```
npm run run:dev
```

### Accéder à l'API :
L'api est accessible sur le port `5678` en local, c'est à dire `http://localhost:5678`

## Lancer le frontend

### Retournez sur le repertoire parent :
```
cd ..
```

### Allez au repo cloné :
```
cd Billed-app-FR-Front
```

### Installez les packages npm (décrits dans package.json) :
```
npm install
```

### Installez live-server pour lancer un serveur local :
```
npm install -g live-server
```

### Lancez l'application :
```
live-server
```
Puis allez à l'adresse : http://127.0.0.1:8080/

## Comment lancer tous les tests en local avec Jest ?
```
npm run test
```

## Comment lancer un seul test ?
### Installez jest-cli :
```
npm i -g jest-cli
jest src/__tests__/your_test_file.js
```

## Comment voir la couverture de test ?
```
http://127.0.0.1:8080/coverage/lcov-report/
```

## Compte et utilisateur :
Vous pouvez vous connecter en utilisant les comptes:
### administrateur : 
```
utilisateur : admin@test.tld 
mot de passe : admin
```
### employé :
```
utilisateur : employee@test.tld
mot de passe : employee
```
