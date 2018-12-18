# Node.js
## npm
```bash
# Publish a public module to the NPM repository
npm publish --access public
```

## List
* [awesome-nodejs-security](https://github.com/lirantal/awesome-nodejs-security) - Awesome Node.js Security resources

## Modules
* [randexp](https://github.com/fent/randexp.js) - Create random strings that match a given regular expression

## Code
* Obtain a PDF file with `node-fetch` and Express.js
```js
let data = await fetch( url );
data = await data.buffer();
res.setHeader( 'Content-Transfer-Encoding', 'binary' );
res.setHeader( 'Content-Type', 'application/octet-stream' );
res.setHeader( 'Content-Disposition', 'attachment; filename=quote.pdf' );
res.send( data );
```
