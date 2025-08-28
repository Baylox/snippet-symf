Lancer un serveur local en arrière plan (TLS auto, .env chargé) :
```bash
symfony server:start -d
```

# Vérifier l’environnement/recettes

Version de la Symfony CLI installée sur ta machine
```bash
symfony -v
```

Liste de tous les composants Symfony présents dans le projet :
```bash
composer show symfony/*
```

Liste les recettes Flex du projet Symfony
```bash
symfony composer recipes
```