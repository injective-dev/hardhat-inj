# Injective EVM Demo Hardhat Project

A demonstration project which show how to compile, deploy, test, verify, and interact
with EVM smart contracts on Injective Testnet.

## Tutorial

WIP - written tutorial coming soon!

## How to use this repo

```shell
# install dependencies
npm install

# compile smart contracts
npx hardhat compile

# deploy smart contracts
npx hardhat run script/deploy.js --network inj_testnet
# copy deployed address from output as use subsequently as SC_ADDRESS

# test smart contracts
npx hardhat test # test on emulated localhost EVM
REPORT_GAS=true npx hardhat test # test on emulated localhost EVM with gas reporting
npx hardhat test --network inj_testnet

# interact with smart contracts via an interactive Javascript REPL
npx hardhat console --network inj_testnet

# verify smart contracts on Blockscout
npx hardhat verify --network inj_testnet ${SC_ADDRESS}

```

## Author

[Brendan Graetz](https://blog.bguiz.com/)

## Licence

MIT
