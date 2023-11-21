# ⌐◨-◨

---

## Setup

```
$ git clone git@github.com:sherlock-audit/2023-09-nounsbuilder.git
$ cd 2023-09-nounsbuilder/nouns-protocol
$ yarn install
$ touch .env
```

Now, edit the `.env` file to contain `ETH_RPC_MAINNET` url for forking.

For example:

```
ETH_RPC_MAINNET=https://eth-mainnet.g.alchemy.com/v2/demo/
```

If using alchemy as above, the `demo` needs to be replaced with your api key to properly run tests.

Now, to run tests, use:
```
$ yarn test
```

