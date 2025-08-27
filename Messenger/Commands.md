Pour lancer les commandes de vérification de la BDD et dump le SQL :
```bash
symfony console doctrine:schema:update --dump-sql 
```

Pour lancer les commandes du worker et afficher les messages :
```bash
symfony console messenger:consume async -vv
```