BIP39 Mnemonics for Bitcore-Innova
=======

A module for [bitcore-innova](https://github.com/innovacoin/bitcore-innova) that implements [Mnemonic code for generating deterministic keys](https://github.com/bitcoin/bips/blob/master/bip-0039.mediawiki).

## Getting Started

This library is distributed in both the npm and bower packaging systems.

```sh
npm install bitcore-mnemonic-innova
bower install bitcore-mnemonic-innova
```

There are many examples of how to use it on the developer guide [section for mnemonic](http://bitcore.io/guide/module/mnemonic/index.html). For example, the following code would generate a new random mnemonic code and convert it to a `HDPrivateKey`.

```javascript
var Mnemonic = require('bitcore-mnemonic-innova');
var code = new Mnemonic(Mnemonic.Words.SPANISH);
code.toString(); // natal hada sutil año sólido papel jamón combate aula flota ver esfera...
var xpriv = code.toHDPrivateKey();
```

## Contributing

See [CONTRIBUTING.md](https://github.com/innovacoin/bitcore-innova/blob/master/CONTRIBUTING.md) on the main bitcore-innova repo for information about how to contribute.

## License

Code released under [the MIT license](https://github.com/bitpay/bitcore/blob/master/LICENSE).

Copyright 2013-2015 BitPay, Inc. Bitcore is a trademark maintained by BitPay, Inc.
