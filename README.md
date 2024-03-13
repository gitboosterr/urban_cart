# React + TypeScript + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## Expanding the ESLint configuration

If you are developing a production application, we recommend updating the configuration to enable type aware lint rules:

- Configure the top-level `parserOptions` property like this:

```js
export default {
  // other rules...
  parserOptions: {
    ecmaVersion: 'latest',
    sourceType: 'module',
    project: ['./tsconfig.json', './tsconfig.node.json'],
    tsconfigRootDir: __dirname,
  },
}
```

- Replace `plugin:@typescript-eslint/recommended` to `plugin:@typescript-eslint/recommended-type-checked` or `plugin:@typescript-eslint/strict-type-checked`
- Optionally add `plugin:@typescript-eslint/stylistic-type-checked`
- Install [eslint-plugin-react](https://github.com/jsx-eslint/eslint-plugin-react) and add `plugin:react/recommended` & `plugin:react/jsx-runtime` to the `extends` list

<!-- node version -->v20.11.0



<!-- folder structure -->

1.assets: Store your static assets like images and styles.

2.components: Reusable components that are not tied to specific features. Common components go in the common folder, while feature-specific components go into their respective folders.

3.config: Configuration files, such as route configurations and API endpoint URLs.

4.containers: Container components that connect to the Redux store. Each feature has its own container.

5.hooks: Custom hooks that can be reused across components and containers.

6.pages: Top-level components for each route. These components should mainly handle the layout and structure of the page.

7.redux: Redux-related files, including actions, reducers, and the Redux store configuration.

8.utils: Utility functions and helper files that don't fit elsewhere.

9.App.js: The main component where routes and layout are defined.

10.index.js: The entry point of your application.

11.This structure separates concerns, promotes reusability, and makes it easier to locate and maintain different parts of your application. Additionally, consider using tools like React Router for handling routes and code splitting for lazy loading to improve performance.

<!-- folder structure end-->
