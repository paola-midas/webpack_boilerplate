# webpack_boilerplate
Webpack 4 config

## Zero configuration ##
The concept of zero configuration in webpack 4 applies to:

* the entry point. Default to ./src/index.js
* the output. Default to ./dist/main.js
* production and development mode (no need to create 2 separate confs for production and development)

## New Module Types ##
Webpack now supports these module types:

* javascript/auto: (The default one in webpack 3) Javascript module with all module systems enabled: CommonJS, AMD, ESM
* javascript/esm: EcmaScript modules, all other module system are not available
* javascript/dynamic: Only CommonJS and, EcmaScript modules are not available
* json: JSON data, it's available via require and import
* webassembly/experimental: WebAssembly modules (currently experimental)

Webpack will look for the .wasm, .mjs, .js and .json extensions in this order.

## References ##

* (Intro:How to webpack 4)[https://www.valentinog.com/blog/webpack-4-tutorial/]
* (What's new in webpack 4)[https://scotch.io/tutorials/whats-new-in-webpack-4#environment-support]