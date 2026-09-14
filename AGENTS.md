# Instructions pour l'IA

Ce projet est un boilerplate simple d'application de bureau Electron avec Vite et TypeScript. Il sert de base pour développer une application sans remplacer sa structure existante.

## Avant de coder

Lire :

- `.ai/context/project.md`
- `.ai/context/architecture.md`
- `.ai/rules/coding.md`
- `.ai/rules/safety.md`

## Agents

Agents disponibles :

- Architecte : analyse et planifie les changements importants.
- Développeur : écrit et modifie le code.
- Reviewer : relit le code et cherche les problèmes.
- Testeur : crée et exécute les vérifications utiles.

Le détail de chaque rôle se trouve dans `.ai/agents/`.

## Skills

Skills disponibles :

- Coding : comprendre, modifier et expliquer le code.
- Testing : choisir et exécuter les vérifications.
- Debugging : reproduire et corriger un problème.
- Documentation : écrire une documentation exacte et simple.

Le détail se trouve dans `.ai/skills/`.

## Contexte

Les informations connues sur le projet se trouvent dans `.ai/context/`. Les conventions existantes sont documentées dans `.ai/context/conventions.md`.

## Workflows

Utiliser `.ai/workflows/feature.md` pour une nouvelle fonctionnalité, `.ai/workflows/bugfix.md` pour une correction et `.ai/workflows/refactor.md` pour une refactorisation.

Pour une nouvelle fonctionnalité :

Comprendre → Planifier → Coder → Tester → Relire

## Règles importantes

- Garder les changements petits.
- Suivre la structure actuelle du projet.
- Ne pas inventer d'architecture.
- Ne pas exposer de secrets.
- Tester les changements importants.
- Lire `.ai/rules/` avant une modification.