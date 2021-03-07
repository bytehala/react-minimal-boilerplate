# react-minimal-boilerplate

No routing, no Jest, no environment variables, no fluff!
Just quick and easy getting started with React using Webpack and Babel

### Getting Started
```bash
git clone git@github.com:bytehala/react-minimal-boilerplate.git
npm install
npm start
```

---
### Making this project from scratch
https://theshravan.net/blog/the-minimal-react-project-setup-using-webpack-and-babel/

#### Step 1: Create project folder, and package.json file in the folder
```bash
mkdir react-minimal-boilerplate
cd react-minimal-boilerplate
npm init -y
```
#### Step 2: Install React and React DOM packages
```bash
npm install --save react react-dom
```
#### Step 3: Install Webpack, Webpack CLI and Webpack Dev Server
```bash
npm install --save-dev webpack
npm install --save-dev webpack-cli
npm install --save-dev webpack-dev-server
```
#### Step 4: Install Babel
```bash
npm install --save-dev @babel/core babel-loader
npm install --save-dev @babel/preset-env @babel/preset-react
```
> The @babel/core is the babel compiler. The babel-loader is the webpack plugin for babel. The @babel/preset-env is the Babel preset for converting ES6, ES7 and ES8 code to ES5. The @babel/preset-react is the Babel preset for all React plugins.

`We have all the required npm packages, let’s write some code. First, we need to create Babel configuration in .babelrc file to tell Babel how to transpile our ES6, ES7, ES8 and JSX code.`
#### Step 5: Create Babel configuration file .babelrc and put this in
```json
{
  "presets": ["@babel/preset-env", "@babel/preset-react"]
}
```
#### Step 6
