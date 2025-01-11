# Prettier Configuration Guide

This repository contains the Prettier configuration file for consistent code formatting across all your projects. By using this configuration, you ensure that your code adheres to a unified style, making collaboration easier and code readability better.

### Install Prettier

To install Prettier as a dev dependency in your project, run the following command:

```bash
npm install prettier -D
```

or

```bash
npm install --save-dev prettier
```

### Running Prettier

Once Prettier is set up in your project, you can use it to format your code. By default, Prettier formats files using its standard formatting rules. However, when you add a .prettierrc file to your project root folder, you can define your own custom formatting rules.

To format all the files in your project according to the rules specified in your .`prettierrc` file, run the following command:

```bash
npx prettier --write .
```

This will format all the files in your project based on the configuration defined in the `.prettierrc` file.

### Check Which Files Need Formatting

If you want to check which files need to be formatted before running the formatting command, you can use the following command:

```bash
npx prettier --check .
```

This will list all the files that are not following the Prettier formatting rules without actually modifying them. Once you've reviewed the files, you can proceed with the --write command to format them.

#### `.prettierrc`

This is the Prettier configuration file. It defines the rules that Prettier will follow to format your code.

```json
{
  "printWidth": 100,
  "tabWidth": 2,
  "useTabs": false,
  "semi": true,
  "singleQuote": false,
  "quoteProps": "consistent",
  "jsxSingleQuote": false,
  "trailingComma": "all",
  "bracketSpacing": true,
  "bracketSameLine": true,
  "arrowParens": "avoid",
  "proseWrap": "preserve",
  "htmlWhitespaceSensitivity": "css",
  "endOfLine": "lf",
  "embeddedLanguageFormatting": "auto"
}
```

#### `.prettierignore`

This file defines the files and directories that Prettier should ignore.

```
node_modules/
dist/
build/
*.min.js
```
