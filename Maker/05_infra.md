# Infra (Console, Events, Messenger)

## Commandes Console
Crée une **commande CLI** avec la structure *execute()* prête : 
```bash
php bin/console make:command <nom:de:commande>
```
> Exemple: 
```bash
php bin/console make:command app:reindex
```
> génère src/Command/ReindexCommand.php.

## Event Subscriber (Kernel / HTTP / Console)
Crée un Event Subscriber (abonné à un ou plusieurs événements). Choisir les events à la génération.
```bash
php bin/console make:event-subscriber
```

> Possibilité d'injecter tes services directement dans les Commandes Console.
---
**Exemples d’événements** utiles :

> Symfony\Component\HttpKernel\Event\RequestEvent (pré-traiter la requête)

> Symfony\Component\HttpKernel\Event\ResponseEvent (ajouter des headers)

> Symfony\Component\Console\Event\ConsoleCommandEvent (pré/ post hooks de commandes)

---

- Préfère les Subscribers (liste explicite des events) aux Listeners isolés pour rester lisible.
- Pour la sécurité, évite toute mutation globale imprévisible (headers/CSP doivent être déterministes).
- Pour Doctrine, utilise plutôt des Lifecycle Callbacks sur entité ou des Subscribers Doctrine dédiés (à coder manuellement ou via un autre fichier maker si tu en as un).

## Messenger (Message & Handler)

Génère une classe de message (simple payload, immuable si possible).
```bash
php bin/console make:message <NomDuMessage>
```

Génère un Message Handler (_consommateur_ , traitement asynchrone/sync selon routing Messenger).
```bash
php bin/console make:message-handler <NomDuHandler>
```

- Route tes messages dans messenger.yaml (ex. transport async).
- Lancement worker : php bin/console messenger:consume <transport.> -vv.
- Sécurité : valide les payloads (DTO stricts), pas de désérialisation d’objets arbitraires.
- Robustesse : configure retry, failure transport et surveille via messenger:failed:*.

