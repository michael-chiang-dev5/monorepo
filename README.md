# monorepo-starter-kit
Implements monorepo described in:
https://dev.to/ynwd/how-to-create-react-monorepo-with-npm-workspace-webpack-and-create-react-app-2dhn

## Instructions
* Clone git repository
* Install dependencies by running `$ npm install` in base monorepo folder
* Create your react app `$ npx create-react-app app1` in `web/modules/`
  * Edit "name" in `package.json`
  `"name": "@mc/app1"`
* Build components from base monorepo folder by running `npm run build -w @mc/components`
* Build react app from base monorepo folder by running `npm start -w @mc/app1`
* Import shared components with `import { ComponentName } from "@mc/components"`

## TODO:
* Consider adding storybook https://dev.to/ynwd/how-to-integrate-storybook-with-npm-workspace-react-and-webpack-4cb5
* There is an error running create-react-app the first time.