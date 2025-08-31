## Sécurité

## Créer un utilisateur
Génère une **entité User** conforme à UserInterface et prête pour l’authentification : 
```bash
php bin/console make:user
```
Posiibilité d'implémenter un User par un autre nom, exemple :
```bash
php bin/console make:user <NomUser>
```

## Créer un voter : 
Génère un Voter (contrôle d’accès fin, ABAC/RBAC) permettant de décider si un utilisateur a le droit d’effectuer une action :
```bash
php bin/console make:voter <NomDuVoter>
```

## Créer une authentification par formulaire
Met en place une authentification classique (login form + sécurité de base) :
```bash
php bin/console make:security:form-login
```
Utilisation d'un authenticator personnalisé :
```bash
php bin/console make:auth
```
## Hasher un mot de passe
Permet de générer un mot de passe hashé :
```bash
php bin/console security:hash-password
```

## Vérifier la config de sécurité
Sert à inspecter la configuration de sécurité du projet.
```bash
php bin/console debug:config security
```