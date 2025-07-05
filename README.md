# Injective EVM Demo Hardhat Project

A demonstration project which show how to compile, test, deploy, verify, and interact
with EVM smart contracts on Injective Testnet.

## Tutorial

This is a demo repo intended to accompany the following series of tutorials:

* [Setup Hardhat and compile a smart contract](https://docs.injective.network/developers-evm/smart-contracts/compile-hardhat)
* [Test a smart contract using Hardhat](https://docs.injective.network/developers-evm/smart-contracts/test-hardhat)
* [Deploy a smart contract using Hardhat](https://docs.injective.network/developers-evm/smart-contracts/deploy-hardhat)
* [Verify a smart contract using Hardhat](https://docs.injective.network/developers-evm/smart-contracts/verify-hardhat)
* [Interact with a smart contract using Hardhat](https://docs.injective.network/developers-evm/smart-contracts/interact-hardhat)

## How to use this repo

```shell
# install dependencies
npm install

# compile smart contracts
npx hardhat compile

# test smart contracts
npx hardhat test # test on emulated localhost EVM
npx hardhat test --network inj_testnet # test on Injective Testnet (not recommended in most cases)

# deploy smart contracts
npx hardhat run script/deploy.js --network inj_testnet
# copy deployed address from output as use subsequently as SC_ADDRESS

# interact with smart contracts via an interactive Javascript REPL
npx hardhat console --network inj_testnet

# verify smart contracts on Blockscout
npx hardhat verify --network inj_testnet ${SC_ADDRESS}

```

## Author

[Brendan Graetz](https://blog.bguiz.com/)

## Licence

MIT
