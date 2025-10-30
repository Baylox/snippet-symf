# Testing

## Tests

Créer un test :
```bash
symfony console make:test
```

Créer un test unitaire :
```bash
symfony console make:unit-test
```

Créer un test fonctionnel :
```bash
symfony console make:functional-test
```

## Lancer les tests

Lancer tous les tests :
```bash
php bin/phpunit
```

Lancer un test spécifique :
```bash
php bin/phpunit tests/Controller/ProductControllerTest.php
```

Lancer avec coverage :
```bash
php bin/phpunit --coverage-html var/coverage
```

## Fixtures de test

Charger les fixtures en environnement test :
```bash
symfony console doctrine:fixtures:load --env=test
```

---

[← Retour](../README.md)
