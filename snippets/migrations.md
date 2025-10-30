# Migrations

## Créer une migration

```bash
symfony console make:migration
```

## Appliquer les migrations

```bash
symfony console doctrine:migrations:migrate
```

Avec confirmation auto :
```bash
symfony console doctrine:migrations:migrate -n
```

## Rollback

Annuler la dernière migration :
```bash
symfony console doctrine:migrations:migrate prev
```

## Status

Voir l'état des migrations :
```bash
symfony console doctrine:migrations:status
```

## Liste

Lister toutes les migrations :
```bash
symfony console doctrine:migrations:list
```

---

[← Retour](../README.md)
