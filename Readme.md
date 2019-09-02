This is a repository made for personal ownt prupose in to learn about how webpack works, and how can I made a project and configure the webpack for it.

Probably will be a lot o language syntax errors, because I made this documentation in english to practice the language, so I'm sorry ^^

This documentation was made using this <a href="https://medium.com/rocketseat/entendendo-e-dominando-o-webpack-4b2e8b3e02da">article</a> and another fonts as reference

## Introductions

There are a lot of concepts inside the webpack module, but for us clients, we need to know about some of their.

### Entry

Entry is a main file that webpack will considerate for make a compact file using all dependencies of this entry file.
Is literally a entry point of your application.

```
module.exports = {
  entry: './path/file.js'
}
```

This is a example of a config that choose the file.js as entry file of your application.

We need to know to, that can be used more than one entry point in your configuration.

### Output

as I said, the webpack build a unique file that englobe all of dependencies of the entry point, and the output of this new file generated by webpack can be configured too in the webpack definitions.

```
const path = require('path');
module.exports = {
  entry: './path/file.js'
  output: {
    path: path.resolve(__dirname, 'dist'),
    filename: 'webpack.bundle.js'
  }
}
```

### Running webpack

To run webpack and build your file, you need to first install webpack using some manager of dependencies (npm, yarn ...).

```
npm i --save webpack
yarn add webpack
```

As default the webpack generate the file in ./dist diretory with the name of entry file.

And after, for simplify the things, we can use the webpack cli to build our application

```
npm i --save-dev webpack-cli
yarn add -D webpack-cli
```

### Configurations

The webpack can be customizated using a .js file that will be contais all informations of the way the webpack will be run.

By default, the webpack looks for a file called webpack.config.js, but you can change this when calling the cli command.

## Webpack for Web

## Webpack for Nodejs
