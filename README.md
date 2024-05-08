
### Switch Back to CommonJS
If you prefer to keep using CommonJS syntax or if your project relies on many CommonJS modules, you can configure Node.js to treat your JavaScript files as CommonJS by changing the "type": "module" in your package.json to "type": "commonjs", or you can remove the "type": "module" line altogether since CommonJS is the default.

If the "type": "module" is necessary for other parts of your application, another solution is to rename your CommonJS files with a .cjs extension. For example, rename server.js to server.cjs.

``` bash
node server.cjs
```
