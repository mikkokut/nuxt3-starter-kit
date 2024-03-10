# Nuxt 3 Starter Kit
Just another Nuxt 3 starter kit.

## Features
- [ESLint](https://eslint.org/)
  - [antfu config](https://github.com/antfu/eslint-config)
  - [eslint-plugin-only-warn](https://github.com/bfanger/eslint-plugin-only-warn)
- [Typecheck](https://nuxt.com/docs/api/configuration/nuxt-config#typecheck) enabled
- [Yarn](https://yarnpkg.com/) as package manager

## Configure VS Code auto fix [*(source)*](https://github.com/antfu/eslint-config?tab=readme-ov-file#vs-code-support-auto-fix)
```json
{
  // Enable the ESlint flat config support
  "eslint.experimental.useFlatConfig": true,

  // Disable the default formatter, use eslint instead
  "prettier.enable": false,
  "editor.formatOnSave": false,

  // Auto fix
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": "explicit",
    "source.organizeImports": "never"
  },

  // Silent the stylistic rules in you IDE, but still auto fix them
  "eslint.rules.customizations": [
    { "rule": "style/*", "severity": "off" },
    { "rule": "format/*", "severity": "off" },
    { "rule": "*-indent", "severity": "off" },
    { "rule": "*-spacing", "severity": "off" },
    { "rule": "*-spaces", "severity": "off" },
    { "rule": "*-order", "severity": "off" },
    { "rule": "*-dangle", "severity": "off" },
    { "rule": "*-newline", "severity": "off" },
    { "rule": "*quotes", "severity": "off" },
    { "rule": "*semi", "severity": "off" }
  ],

  // Enable eslint for all supported languages
  "eslint.validate": [
    "javascript",
    "javascriptreact",
    "typescript",
    "typescriptreact",
    "vue",
    "html",
    "markdown",
    "json",
    "jsonc",
    "yaml",
    "toml"
  ]
}
```

## Start development server
```bash
yarn dev
```
