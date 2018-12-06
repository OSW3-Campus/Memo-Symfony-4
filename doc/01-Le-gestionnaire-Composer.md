> # Le gestionnaire **Composer**
Composer est un gestionnaire de dépendances, libre, écrit en PHP.  
Avec Symfony, **Composer** est un outil essentiel pour la création, la mise à jour et la mise en production du projet.  
Il permet également l'ajout de librairie externe au projet.


# Installer Composer

## Installer composer pour Linux et MacOS

Pour installer Composer, copier ces quelques ligne dans votre Terminal.
```
php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"
php -r "if (hash_file('SHA384', 'composer-setup.php') === '93b54496392c062774670ac18b134c3b3a95e5a5e5c8f1a9f115f203b75bf9a129d5daa8ba6a13e2cc8a1da0806388a8') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"
php composer-setup.php
php -r "unlink('composer-setup.php');"
```

1. PHP copie le fichier d'installation de Composer sur votre machine.
2. PHP vérifie l'intégrité du fichier composer-setup.php.
3. PHP exécute le fichier composer-setup.php qui procèede à l'installation de Composer.
4. PHP supprime le fichier composer-setup.php devenu inutile.

## Installer Composer pour Windows

Télécharger et exécuter le fichier Composer-Setup.exe (téléchargement depuis le site officiel de Composer.)


# Commandes essentielles

### Version de Composer
```
composer -v
```

**Mise à jour de composer**
```
composer self-update
```

**Installation d'un projet**
Installe / Initialise un projet après récupération des sources.
```
composer install
```

**Mise à jour des composants d'un projet**
```
composer update
```

**Ajout d'un composant**
Ajoute un composant au projet.

La dépendance du composant sera inscrite dans le fichier `composer.json`.
```
composer require source-du-composant
```

Ajoutez l'option `--dev` pour un composant utilisé uniquement pendant le développement du projet.
```
composer require source-du-composant --dev
```


# Liens

- [Site officiel​](https://getcomposer.org/)
- [Composer sur Wikipédia​](https://fr.wikipedia.org/wiki/Composer_(logiciel))
- [Composer sur GitHub​](https://github.com/composer/composer)