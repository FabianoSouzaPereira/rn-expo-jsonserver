## Created based on the Expo project create react-native-app

Created project with the command:

yarn create react-native-app

## Present Features from the Expo

- Native project ready to be built on to your device.
- Support for unimodules and auto-linking.
- OTA updates, and Gestures out of the box.
- Full support for React Native web.
- Plug-n-play custom templates.
- Works with the Expo Client app.

## Features add in the project;

    yarn add json-server
    yarn add eslint-config-prettier
    	yarn add --dev --exact prettier
    	yarn add --dev prettier

## Start Json Server

Create a db.json file with some data

    {
    "posts": [
        { "id": 1, "title": "json-server", "author": "typicode" }
    ],
    "comments": [
        { "id": 1, "body": "some comment", "postId": 1 }
    ],
    "profile": { "name": "typicode" }
    }

json-server --watch db.json

Navigador: server ip http://localhost:3000

In emulator: http://10.0.2.2:3000

Details on https://www.npmjs.com/package/json-server

## Typescritp with types

yarn add --dev typescript @types/react @types/react-native @types/react-dom @tsconfig/react-native

Add to your tsconfig.json:

    "extends": "@tsconfig/react-native/tsconfig.json"

### Scripts for Typescrip

    create tsconfig.json: {
        "compilerOptions": {
        "allowSyntheticDefaultImports": true,
        "jsx": "react-native", "lib": ["dom", "esnext"],
        "moduleResolution": "node",
        "noEmit": true,
        "skipLibCheck": true,
        "resolveJsonModule": true,
        "strict": true }
        }

File package.json

    "scripts": {
        ... "tsc:w": "tsc --watch"
    },

Rename files to convert them to TypeScript. For example, you would rename App.js to App.tsx.

Use the .tsx extension if the file includes React components (JSX). If the file did not include any JSX, you can use the .ts file extension.

## Redux types

yarn add @types/react-redux

## Extra facilities

Source code organization was added to the elslint and Pretter project.

Find Problems ESLint statically analyzes your code to quickly find problems. ESLint is built into most text editors and you can run ESLint as part of your continuous integration pipeline.

Fix Automatically Many problems ESLint finds can be automatically fixed. ESLint fixes are syntax-aware so you won't experience errors introduced by traditional find-and-replace algorithms.

Customize Preprocess code, use custom parsers, and write your own rules that work alongside ESLint's built-in rules. You can customize ESLint to work exactly the way you need it for your project.

    INSTALL ESLINT to help organize the code https://eslint.org/

    1. Install extentions to VSCODE eslint

    2. After install on teminal

    	yarn add eslint --dev
    	yarn eslint --init

    	 obs.: answer questions

    3. INSTALL PRETTY to work together with eslint  https://prettier.io/

    	yarn add --dev --exact prettier
    	yarn add --dev prettier

    4. Install extentions to VSCODE   ESLint 2.1.8

    5. After to Install

    	In .eslintrc.json:

    	{
    	  "plugins": ["prettier"],
    	  "rules": {
    	    "prettier/prettier": "error"
    	  }
    	}

    	Run prettier on the entire project to format everything:

    	  yarn prettier --write .

    6. After install:

    	yarn add eslint-config-prettier

    	Then you need to add plugin:prettier/recommended as the last extension in your .eslintrc.json:

    	{
    	  "extends": ["plugin:prettier/recommended"]
    	}


    7. Run Typescript on the entire project to format everything:

    	yarn tsc


    8. .eslintrc.json:

        "rules": {
        "semi": [
            "warn",
            "always"
        ],
        "quotes": [
            "warn",
            "single"
        ],
        "no-unused-vars": "off",
        "@typescript-eslint/no-unused-vars": [
            "off"
        ],
        "@typescript-eslint/explicit-module-boundary-types": "off",
        "overrides": [
            {
                // enable the rule specifically for TypeScript files
                "files": [
                    "*.ts",
                    "*.tsx"
                ]
            }
        ]
    }

## Axios

- Make XMLHttpRequests from the browser
- Make http requests from node.js
- Supports the Promise API
- Intercept request and response
- Transform request and response data
- Cancel requests
- Automatic transforms for JSON data
- Client side support for protecting against XSRF

  yarn add axios @types/axios

### Links

    https://www.typescriptlang.org/
    https://eslint.org/
    https://prettier.io/
    https://www.npmjs.com/package/json-server
