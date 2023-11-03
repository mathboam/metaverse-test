# React + TypeScript + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## Expanding the ESLint configuration

If you are developing a production application, we recommend updating the configuration to enable type aware lint rules:

- Configure the top-level `parserOptions` property like this:

```js
   parserOptions: {
    ecmaVersion: 'latest',
    sourceType: 'module',
    project: ['./tsconfig.json', './tsconfig.node.json'],
    tsconfigRootDir: __dirname,
   },
```

- Replace `plugin:@typescript-eslint/recommended` to `plugin:@typescript-eslint/recommended-type-checked` or `plugin:@typescript-eslint/strict-type-checked`
- Optionally add `plugin:@typescript-eslint/stylistic-type-checked`
- Install [eslint-plugin-react](https://github.com/jsx-eslint/eslint-plugin-react) and add `plugin:react/recommended` & `plugin:react/jsx-runtime` to the `extends` list

<!-- Application Configuration -->

To start the application locally, the development packages have to be installed by navigating to the application folder on your command prompt(Terminal on mac) and running the command below.

yarn install
or
yarn

A .env file is also needed to run this application.
Create a .env file at the root level of the repository.
Inside the .env file, add the text below.

VITE_SOCKET_URL=wss://frontend-test-api.mvm-tech.xyz/ws?token=
VITE_API_URL=https://frontend-test-api.mvm-tech.xyz/api/

This will provide the application with the neccessary environment variables.

After that, run the below command in your terminal to start the application locally

yarn dev
