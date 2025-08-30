# Entités & Database

## Créer une entité Doctrine
**Crée une entité** (classe mappée sur une table de la BDD) avec ses propriétés.

```bash
php bin/console make:entity <NomDeLEntité>
```

## Générer une migration

Analyse les différences entre entités PHP et la base de données, puis **crée une migration** :

```bash
php bin/console make:entity <NomDeLEntité>
```
## Exécuter les migrations

Applique les migrations en attente à la base de données:
```bash
php bin/console doctrine:migrations:migrate
```
Avec confirmation auto :

```bash
php bin/console doctrine:migrations:migrate -n
```
## Charger des fixtures

Crée une **classe de fixtures** :
```bash
php bin/console make:fixtures <NomDesFixtures>
```
**Charge les fixtures** dans la BDD :
```bash
php bin/console doctrine:fixtures:load
```
Avec **rechargement automatique** (purge + reload sans poser de questions) :
```bash
php bin/console doctrine:fixtures:load -n
```

**Charge Factory/Story** dans la BDD :
```bash
php bin/console foundry:load-fixtures
```

## Vérifier la synchronisation du schéma
**Valide** que les entités et la base sont cohérentes.
```bash
php bin/console doctrine:schema:validate
```