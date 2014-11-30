# Grrr ! les traches automtisées de grunt

![Grunt](../images/grunt.jpg)

## Qu'est-ce que c'est que ce truc ?

[Grunt](Grunt: The JavaScript Task Runner - Gruntjs) est un lanceur de taches automatisées écrit en javascript.
Tout un programme !

<img src="../images/Troll-face.jpg" width="50" alt="Troll time" title="Troll time" /> Allergiques à la ligne de commande : fuyez !

## Installation de node.js

Sur OSX :
```sh
brew install node
```

## Installation de grunt

```sh
npminstall -g grunt-cli
```

## Transpilation

```sh
cd bootstrap/
```

Installer les modules nécessaires au projet local

```sh
npm install
```

Ceci fait, vous êtes capable de lancer les taches suivantes :

- `grunt dist` Déploiement unique
- `grunt watch` Déploiement et processus de recompilation automatique
- `grunt test` Lancement des tests de mise en production
- `grunt docs` Déploiement de la documentation
- ` grunt` Active le lancement de toutes les taches

