# Architecture

- `electron/main.ts` est le point d'entrée du processus principal Electron et crée la fenêtre.
- `electron/preload.ts` contient le script de préchargement.
- `src/main.ts` est le point d'entrée du renderer et construit l'interface.
- `src/counter.ts` contient la logique du compteur d'exemple.
- `src/style.css` contient les styles du renderer.
- `index.html` fournit la page HTML chargée par Vite.
- `public/` contient les ressources publiques utilisées par l'application.
- `vite.config.ts` configure Vite et les entrées Electron.
- `dist/`, `dist-electron/` et `release/` contiennent des sorties générées ou empaquetées.

La configuration de débogage existante se trouve dans `.vscode/`. Elle lance la tâche `Before Debug` puis les processus principal et renderer.