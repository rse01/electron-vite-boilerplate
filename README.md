# electron-vite-boilerplate

🥳 Un boilerplate `Electron` + `Vite` vraiment simple.

![screenshort.png](https://github.com/electron-vite/electron-vite-boilerplate/blob/main/public/screenshort.png?raw=true)

## Fonctionnalités

📦 Prêt à l'emploi  
🚀 Démarrage rapide avec [vite-plugin-electron](https://github.com/electron-vite/vite-plugin-electron)  
🎯 Basé sur le template officiel [template-vanilla-ts](https://github.com/vitejs/vite/tree/main/packages/create-vite/template-vanilla-ts), peu invasif

## Mise en route

```sh
# cloner le projet
git clone https://github.com/electron-vite/electron-vite-boilerplate.git

# entrer dans le dossier du projet
cd electron-vite-boilerplate

# installer les dépendances
npm install

# développer
npm run dev
```

## Directory

```diff
+ ├─┬ electron
+ │ ├─┬ main
+ │ │ └── index.ts    point d'entrée du processus principal Electron
+ │ └─┬ preload
+ │   └── index.ts    point d'entrée des scripts de préchargement
  ├─┬ src
  │ └── main.ts       point d'entrée du processus de rendu Electron
  ├── index.html
  ├── package.json
  └── vite.config.ts
```

## Be aware

🚨 Par défaut, ce template intègre Node.js dans le processus de rendu. Si vous n'en avez pas besoin, vous juste enlever l'option ci-dessous. [Parce que cela modifiera la configuration par défaut de Vite](https://github.com/electron-vite/vite-plugin-electron/tree/main/packages/electron-renderer#config-presets-opinionated).

```diff
# vite.config.ts

electron({
- renderer: {}
})
```

## FAQ

- [dependencies vs devDependencies](https://github.com/electron-vite/vite-plugin-electron/tree/main/packages/electron-renderer#dependencies-vs-devdependencies)
- [Using C/C++ native addons in Electron-Renderer](https://github.com/electron-vite/vite-plugin-electron/tree/main/packages/electron-renderer#load-nodejs-cc-native-modules)
- [Node.js ESM packages](https://github.com/electron-vite/vite-plugin-electron/tree/main/packages/electron-renderer#nodejs-esm-packages) (e.g. `execa` `node-fetch`)
