> # Créer une Entité
Une Entité est une Classe PHP qui vous permet de générer les tables et champs de base de données, les formulaires et contrôles de formulaires lors de l'envois des données.


# Créer une Entité

On créer l'entité `Books`. Par la suite, le nom de l'entité sera attribué à la table `Books` de la base de données.

```bash
php bin/console make:entity Books
```


# Ajouter des propriétés

Une fois l'entité crée, le Terminal nous propose d'ajouter les propriétés. Les propriétés deviendront ensuite les champs de la table `Books`.

## Nom de la propriété

```bash
New property name (press <return> to stop adding fields):
> title
```

Nous avons saisi `title`, qui représentera le titre d'un livre.

## Type de la propriété

```bash
Field type (enter ? to see all types) [string]:
>
```

Par défaut, la propriété sera de type **string**. Si vous validez (touche entré) sans saisir de type, le type par défaut s'appliquera.

Pour connaitre tous les types possible, vous devez saisir un point d'interrogation.

## Longueur / Taille de la propriété

```bash
Field length [255]:
>
```

Par défaut, une propriété de type string aura une taille de 255 caractères. Si vous validez (touche entré) sans modifier la taille, la taille par défaut s'appliquera.

## Champ à valeur nulle ?

```bash
Can this field be null in the database (nullable) (yes/no) [no]:
>
```

Par défaut, le champ de la base de données ne pourra pas être nulle. Si vous souhaitez autoriser que ce champ ne possède pas de valeur, vous pouvez saisir yes.

Ajouter des propriétés sur une Entité existante
Pour ajouter des propriétés sur une entité existante, il suffit de saisir la même commande que pour la création de cette entité.

Le Terminal vous avertira que l'entité existe déjà et vous proposera d'ajouter les nouvelles propriétés 

```bash
php bin/console make:entity categories
```


# Mise à jour de Getters / Setters

```bash
php bin/console make:entity --regenerate
```

Cette commande ne supprime pas les Getters / Setters des propriété supprimées.


# Créer une Entité depuis une table existante

Générer l'entité en PHP avec annotation :

```bash
php bin/console doctrine:mapping:import 'App\Entity' annotation --path=src/Entity
```

Générer l'entité en XML :

```bash
php bin/console doctrine:mapping:import 'App\Entity' xml --path=config/doctrine
```


# Créer le Repository associé à l'Entité
Assurer vous que l'Entité possède la ligne d'annotation suivante :

```php
/**
 * @ORM\Entity(repositoryClass="App\Repository\MyClassRepository")
 */
class MyClass
{
}
```

Puis exécuter la commande :

```bash
php bin/console make:entity --regenerate
```


## Types de champs

### Général

```text
string
text
boolean
integer (or smallint, bigint)
float
```

### Relations / Associations

```text
relation (a wizard will help you build the relation)
ManyToOne
OneToMany
ManyToMany
OneToOne
```

### Tableaux / Objets

```text
array (or simple_array)
json
object
binary
blob
```

### Date / Heure

```text
datetime (or datetime_immutable)
datetimetz (or datetimetz_immutable)
date (or date_immutable)
time (or time_immutable)
dateinterval
```

### Autres

```text
json_array
decimal
guid
```
​

