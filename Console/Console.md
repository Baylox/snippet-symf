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
