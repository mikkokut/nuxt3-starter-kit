# Nuxt 3 Starter Kit
Just another Nuxt 3 starter kit.

## Features
- [ESLint](https://eslint.org/) 
  - [antfu config](https://github.com/antfu/eslint-config)
  - [eslint-plugin-only-warn](https://github.com/bfanger/eslint-plugin-only-warn)
- [Typecheck](https://nuxt.com/docs/api/configuration/nuxt-config#typecheck) enabled
- [Yarn](https://yarnpkg.com/) as package manager


## Configure VS Code auto fix [*(source)*](https://github.com/antfu/eslint-config#config-vs-code-auto-fix)
```json
{
  "prettier.enable": false,
  "editor.formatOnSave": false,
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": true
  }
}
```

## Start development server
```bash
yarn dev
```
