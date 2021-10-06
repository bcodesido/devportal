---
layout: rsk
title: rLogin - Migrating
---

The rLogin has ease migration process from other libraries

### Web3modal

The Web3modal configuration will be completely compatible with rLogin configuration. The only required change is

```diff=
- web3modal.connect().then(provider => {})
+ rLogin.connect().then(({ provider }) => {})
```

### Web3 React

Use the [`rsksmart/rLogin-web3-react-connector` adapter](https://github.com/rsksmart/rLogin-web3-react-connector) to ingtegrate rLogin on top of web3 React