# Eslint and Prettier Setup

These are my settings for eslint and prettier

## What it does

- Lints JavaScript based on the latest standards
- Fixes issues and formatting errors with Prettier
- Lints + Fixes inside of html script tags
- You can see all the [rules here](https://github.com/jhanikhilnath/eslint-config-nikhil/blob/master/.eslintrc.json) - I follow these rules All the Time. You are welcome to change anything you don't like

## Installing

I will show you how to install the package locally and in each project as it is the best way to customize it on prject level.

### Locally

1. If you don't already have a `package.json` file, create one with `npm init`.

2. Then we need to install everything needed by the config:

```
npx install-peerdeps --dev eslint-config-nikhil
```

npx is not a misspelling of npm its a built in tool

3. You can see in your package.json there are now a big list of devDependencies.

4. Create a `.eslintrc.json` file in the root of your project's directory (it should live where package.json does). Your `.eslintrc.json` file should look like this:

```json
{
  "extends": ["nikhil"]
}
```

#### VS Code Setup

You Can install [eslint extention](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint) and [prettier extention](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode) these extentions allow you to:-

1. Eslint extention shows all the errors in VS Code problems Window and underlines them

2. Prettier Extention allows you to format your code inside VS Code

Add this to your settings.json file(or search in settings GUI)

```
"editor.formatOnSave": true
```

---

This project was inspired by [eslint-config-wesbos](https://github.com/wesbos/eslint-config-wesbos).
