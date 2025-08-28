# Lister/chercher une route

Affiche toutes les routes enregistrées du projet:
```bash
composer show symfony/*
```

Cible une route précise par son nom:
```bash
php bin/console debug:router <nom_de_route>
```

# Générer un controller, commande, form, etc.

Crée un **controller** avec une action et la vue Twig associée :
```bash
php bin/console make:controller <NomDuController>
```

Génère une **commande Console** prête à implémenter avec la classe et la configuration de base :
```bash
php bin/console make:command <nom:de:commande>
```

Crée une **classe de formulaire** :
```bash
php bin/console make:form <NomDuFormType>
```
Génère une **contrainte de validation personnalisée**:
```bash
php bin/console make:validator <NomDeLaContrainte>
```

Crée un **Event Subscriber** :
```bash
php bin/console make:event-subscriber
```

Génère un **Twig Component** avec sa classe PHP et son template Twig :
```bash
php bin/console make:twig-component <Chemin/Composant>
```