# Routing & Controllers

## Routes

Lister toutes les routes :
```bash
symfony console debug:router
```

Chercher une route spécifique :
```bash
symfony console debug:router app_home
```

Tester une URL :
```bash
symfony console router:match /api/products/123
```

## Controllers

Créer un controller :
```bash
symfony console make:controller ProductController
```

## CRUD

Créer un CRUD complet :
```bash
symfony console make:crud Product
```

## Forms

Créer un FormType :
```bash
symfony console make:form ProductType
```

## Validation

Créer une contrainte de validation personnalisée :
```bash
symfony console make:validator UniqueEmail
```

## Event Subscribers

Créer un Event Subscriber :
```bash
symfony console make:subscriber
```

## Twig

Créer un composant Twig :
```bash
symfony console make:twig-component Alert
```

Créer une extension Twig :
```bash
symfony console make:twig-extension
```

---

[← Retour](../README.md)
