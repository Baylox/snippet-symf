# Symfony Snippets

> Quick reference pour les commandes Symfony les plus utilisées

[![Symfony](https://img.shields.io/badge/Symfony-7.x-black)](https://symfony.com/)

## Quick Start

# Server
```bash
symfony serve
```

# Entity + Migration
```bash
symfony console make:entity Product
symfony console make:migration
symfony console doctrine:migrations:migrate
```
# Controller
```bash
symfony console make:controller ProductController
```

## Documentation

| Module | Description |
|--------|-------------|
| [Entities](snippets/entities.md) | Entities, schema validation |
| [Migrations](snippets/migrations.md) | Create, apply, rollback migrations |
| [Database](snippets/database.md) | Database creation, drop |
| [Fixtures](snippets/fixtures.md) | Fixtures, Foundry factories |
| [Security](snippets/security.md) | Authentication, authorization, users, voters |
| [Routing](snippets/routing.md) | Routes, controllers, requests/responses |
| [Forms](snippets/forms.md) | Forms, validation, custom constraints |
| [Console](snippets/console.md) | CLI commands, debugging tools |
| [Messenger](snippets/messenger.md) | Async messages, workers, queues |
| [Testing](snippets/testing.md) | Unit tests, functional tests |
| [Debug](snippets/debug.md) | Debug tools, profiler, container inspection |

## Liens utiles

- [Documentation Symfony](https://symfony.com/doc/current/index.html)
- [Symfony CLI](https://symfony.com/download)
- [SymfonyCasts](https://symfonycasts.com/)
