> # Les dépendances essentielles
Liste et description des dépendances essentielles pour un projet Symfony.


# Web Server Bundle

WebServerBundle permet de démarrer le serveur web interet de PHP directement sur le projet Symfony

``` 
composer require symfony/web-server-bundle --dev
``` 

- Source sur [Packagist]() ou [GitHub​]()
- Documentation sur [Symfony​](https://symfony.com/doc/current/setup/built_in_web_server.html)


# Symfony MakerBundle

MakerBundle vous aide pour la création de vos commands, controllers, form classes, tests, ...

``` 
composer require symfony/maker-bundle --dev
``` 

- Source sur [Packagist]() ou [GitHub​]()
- Documentation sur [Symfony​](https://symfony.com/doc/current/bundles/SymfonyMakerBundle/index.html)


# Doctrine

Gestion de la base de données.

``` 
composer require symfony/orm-pack
``` 

- Source sur [Packagist]() ou [GitHub​]()
- Documentation sur [Symfony​]()
- Configuration sur [Symfony​]()


# Extra Bundle

Gestion des annotations dans les contrôleurs 

``` 
composer require sensio/framework-extra-bundle
``` 

# Surcharge de la configuration Apache (.htaccess)

Gestion de la ré-écriture des URL.

``` 
composer require symfony/apache-pack
``` 

- Source sur [Packagist]() ou [GitHub​]()
- Documentation sur [Symfony​]()


# Data Fixtures

Ajouter de fausse données dans la base de données.

``` 
composer require orm-fixtures --dev
``` 

- Source sur [Packagist]() ou [GitHub​]()
- Documentation sur [Symfony​]()


# Fake Data

Générateur de fausses données.

``` 
composer require fzaninotto/faker --dev
``` 

- Source sur [GitHub​](https://github.com/fzaninotto/Faker)


# Security Bundle

Le composant Sécurité fournit un système de sécurité complet pour votre application Web.  
Il est livré avec des fonctionnalités d'authentification via l'authentification de base HTTP, la connexion de formulaire interactive ou la connexion de certificat X.509, mais vous permet également de mettre en œuvre vos propres stratégies d'authentification. En outre, le composant fournit des moyens d'autoriser les utilisateurs authentifiés en fonction de leurs rôles.

``` 
composer require security
``` 

- Source sur [Packagist](https://packagist.org/packages/symfony/security)
- Source sur [GitHub​](https://github.com/symfony/security)
- Documentation sur [Symfony​](https://symfony.com/doc/current/components/security.html)


# Swift Mailer

Envois de mail.

```
composer require symfony/swiftmailer-bundle
```
