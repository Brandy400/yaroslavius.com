Yaroslavius.com
=========
Building
--------

```bash
npm install
npm run dev
# Open localhost:4003/index-dev.html in your browser
```
If the below error occurs
--------
```js
  opensslErrorStack: [ 'error:03000086:digital envelope routines::initialization error' ],
  library: 'digital envelope routines',
  reason: 'unsupported',
  code: 'ERR_OSSL_EVP_UNSUPPORTED'
```
Solution
--------
```bash
set NODE_OPTIONS=--openssl-legacy-provider
```

Building for Production
--------

```bash
npm run build
```