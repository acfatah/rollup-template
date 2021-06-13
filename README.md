# rollup-template

A template to publish ES6 modules to npm.

This template is based on [rollup-starter-lib](https://github.com/rollup/rollup-starter-lib/blob/babel).

## Getting started

Use as template or clone this repository:

```bash
git clone https://github.com/acfatah/rollup-template && \
cd rollup-template && \
npm install
```

`npm run build` builds the library to `dist`, generating three files:

* `dist/cjs/index.js`
    A CommonJS bundle, suitable for use in Node.js, that `require`s the external dependency. This corresponds to the `"main"` field in package.json
* `dist/esm/index.js`
    an ES module bundle, suitable for use in other people's libraries and applications, that `import`s the external dependency. This corresponds to the `"module"` field in package.json
* `dist/umd/index.js`
    a UMD build, suitable for use in any environment (including the browser, as a `<script>` tag), that includes the external dependency. This corresponds to the `"browser"` field in package.json

`npm run dev` builds the library, then keeps rebuilding it whenever the source files change using [rollup-watch](https://github.com/rollup/rollup-watch).


## License

[MIT](LICENSE).
