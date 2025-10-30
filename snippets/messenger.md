# Messenger (Async)

## Messages & Handlers

Créer un message :
```bash
symfony console make:message SendEmailMessage
```

Créer un handler :
```bash
symfony console make:message-handler
```

## Workers

Lancer un worker :
```bash
symfony console messenger:consume async -vv
```

Lancer avec limite de messages :
```bash
symfony console messenger:consume async --limit=10
```

Lancer avec time limit :
```bash
symfony console messenger:consume async --time-limit=3600
```

## Messages en échec

Voir les messages en échec :
```bash
symfony console messenger:failed:show
```

Réessayer les messages en échec :
```bash
symfony console messenger:failed:retry
```

Réessayer un message spécifique :
```bash
symfony console messenger:failed:retry 1
```

Supprimer un message en échec :
```bash
symfony console messenger:failed:remove 1
```

## Stats

Voir les stats du transport :
```bash
symfony console messenger:stats
```

## Configuration

Exemple de configuration dans `.env` :
```bash
MESSENGER_TRANSPORT_DSN=doctrine://default
```

## Diagrammes

![Message Flow](../assets/messenger-flow.png)

---

**Note** : Les messages sont stockés en BDD jusqu'à ce qu'un worker les consomme. Il faut au minimum 2 applications : une qui produit les messages, une qui les consomme.

---

[← Retour](../README.md)
