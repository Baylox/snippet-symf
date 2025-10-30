# Security

## User Entity

Créer une entité User :
```bash
symfony console make:user
```

Créer avec un nom personnalisé :
```bash
symfony console make:user Admin
```

## Authentication

Authentification par formulaire (login form classique) :
```bash
symfony console make:security:form-login
```

Authenticator personnalisé :
```bash
symfony console make:auth
```

## Voters

Créer un Voter (contrôle d'accès fin) :
```bash
symfony console make:voter PostVoter
```

## Password

Hasher un mot de passe :
```bash
symfony console security:hash-password
```

## Debug

Inspecter la configuration de sécurité :
```bash
symfony console debug:config security
```

Vérifier les firewalls :
```bash
symfony console debug:firewall
```

---

[← Retour](../README.md)
