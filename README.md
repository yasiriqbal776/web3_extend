# web3_extended


A simple extension of the web3 interface to access the Management API. 

## Installation

``` bash
  $ npm install web3_extend --save
```

## Usage
Call just as you would normal web3. There is an options object to include. The currently implemented interfaces are personal, admin, and debug. Follows the same function arguments as the Javascript Console reference: [here][0]

**Note:** The security of this module has not been tested. Ideal for working inside a private network or testnet. 

**Example**
```
var web3_extend = require('web3_extend');

var options = {
  host: 'http://localhost:8545',
  personal: true, 
  admin: true,
  debug: false
};
var web3 = web3_extend.create(options);

var datadir = web3.admin.datadir();
//'/Users/username/Library/Ethereum'
```

## Tests

No tests are included

#### License: MIT
#### Author: [yasir Iqbal](https://github.com/yasiriqbal776)

[0]: https://github.com/ethereum/go-ethereum/wiki/JavaScript-Console#admin

Credit :  Jordan Paul(https://github.com/The18thWarrior)
