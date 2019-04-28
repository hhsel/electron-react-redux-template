# Electron React Redux Template
This repository is just for my quick starting point, adjusting to my preferences.  
It could be useful if your preference is similar to mine.

## How to use
```
npm install
```
Then start building, and watch for further changes
```
npm run watch
```
After successfully built, you can start your application
```
npm run start
```
Or you just double-click on .bat files (if you use Windows 10)

## Packages
React Redux, with Material-UI as the UI framework and react-router for routing.  
Built with webpack, babel, and syntax is enforced by ESLint with airbnb extension rules (but some rules are intentionally disabled, noted below)

## Configurations
### ESLint
Based on airbnb rules, but some rules are intentionally disabled.  
See ``.eslintrc.js`` for details.

- semi: ["off"]
  - Semicolons are verbose and just makes code looks worse, when ASI exists in the language. I believe this should not be required.
- react/jsx-filename-extension: ["off"]
  - I prefer to put completely reusable pure JavaScript (framework-independent) files into distinct folders. I believe using two extensions is unnecessary.
- indent: ["error", 4]
  - The indent of 2 is so narrow that I cannot understand my codes quickly.
### webpack
See ``webpack.config.js`` for details.
- Aliases are used. Prefixed with @ to indicate aliases.
  - @actions - Redux action and action creators
  - @stores - Redux stores
  - @reducers - Redux reducers
  - @containers - React Redux container components
  - @components - Ordinary React components

## Directory structure
I don't always use this. I believe this is more suitable for smaller applications.  
For larger ones, it would be better to organize by routing paths first, instead of grouping by roles, like this.  
