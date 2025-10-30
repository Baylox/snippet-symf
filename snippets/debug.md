# Debug Tools

## Container

Lister tous les services :
```bash
symfony console debug:container
```

Chercher un service :
```bash
symfony console debug:container validator
```

Voir les services privés :
```bash
symfony console debug:container --show-private
```

## Autowiring

Voir l'autowiring disponible :
```bash
symfony console debug:autowiring
```

Chercher un type spécifique :
```bash
symfony console debug:autowiring Mailer
```

## Configuration

Voir la configuration complète :
```bash
symfony console debug:config
```

Voir la config d'un bundle :
```bash
symfony console debug:config framework
```

## Events

Lister les event listeners :
```bash
symfony console debug:event-dispatcher
```

Voir les listeners d'un event spécifique :
```bash
symfony console debug:event-dispatcher kernel.request
```

## Twig

Lister les functions/filters Twig :
```bash
symfony console debug:twig
```

## Routes

Lister toutes les routes :
```bash
symfony console debug:router
```

Détails d'une route :
```bash
symfony console debug:router app_home
```

## Messenger

Debug Messenger :
```bash
symfony console debug:messenger
```

## Environment

Vérifier les requirements :
```bash
symfony check:requirements
```

Vérifier les vulnérabilités de sécurité :
```bash
symfony check:security
```

---

[← Retour](../README.md)
