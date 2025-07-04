# Injective EVM Demo Hardhat Project

## How to use this repo

```shell
npm install

npx hardhat help

npx hardhat compile

npx hardhat run script/deploy.js --network inj_testnet
# copy deployed address from output as use subsequently as SC_ADDRESS

npx hardhat test
REPORT_GAS=true npx hardhat test
npx hardhat test --network inj_testnet

npx hardhat console --network inj_testnet

npx hardhat verify --network inj_testnet ${SC_ADDRESS}

```
