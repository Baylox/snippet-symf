# Console Commands

## Commandes

Lister toutes les commandes :
```bash
symfony console
```

Créer une commande personnalisée :
```bash
symfony console make:command app:reindex
```

Voir l'aide d'une commande :
```bash
symfony console help make:entity
```

## Auto-completion

Générer le script d'auto-completion :
```bash
symfony console completion bash > completion.sh
```

## Server

Démarrer le serveur :
```bash
symfony server:start
```

Démarrer en arrière-plan :
```bash
symfony server:start -d
```

Arrêter le serveur :
```bash
symfony server:stop
```

## Cache

Vider le cache :
```bash
symfony console cache:clear
```

Vider le cache de prod :
```bash
symfony console cache:clear --env=prod
```

Préchauffer le cache :
```bash
symfony console cache:warmup
```

## Composer

Voir les recipes installés :
```bash
symfony composer recipes
```

Voir les dépendances Symfony :
```bash
composer show symfony/*
```

---

[← Retour](../README.md)
