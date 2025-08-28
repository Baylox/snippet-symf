Pas besoin de donner la commande par défaut sur Linux (bin/console - fichier éxécutable), sur Windows c'est php bin/console.

Pour avoir la liste des commandes: 

```bash
symfony console
```

On a plus besoin d'humain pour les commandes, permet d'automatiser certains traitements

Hashé un mot de passe :
```bash
symfony console security:hash
```
```bash
$2y$13$SSivz.hWuuYeYCo/MFDDcer1EQVYhknWF3YcVN1UX6U7xKXcQL9wq

$2y$ -> bcrypt ici, c'est le type de hashage
$13$ -> option (coût valeur numérique)
```
Permet de créer une commande: 
```bash
symfony console make:command 
```

Accès au script auto-completion
```bash
php bin/console completion bash > completion.sh
```

## Doctrine
Voir ce que l'update va créer comme requêtes SQL
```bash
symfony console d:s:u --dump-sql
```

Force l'update du mapping Doctrine (NE PAS FAIRE EN PROD)
```bash
symfony console d:s:u --force
```

# Twig
Pour créer un componant
```bash
symfony console make:twig-comp
```
 # Symfony
 Debug - Container, router etc.
 Différence de schéma - Gestion de la conf Doctrine (Doc schema validate et update)

 