# Supply chain & data auditing

This repository containts an Ethereum DApp that demonstrates a Supply Chain flow between a Seller and Buyer. The user story is similar to any commonly used supply chain process. A Seller can add items to the inventory system stored in the blockchain. A Buyer can purchase such items from the inventory system. Additionally a Seller can mark an item as Shipped, and similarly a Buyer can mark an item as Received.

The DApp User Interface when running should look like...

![truffle test](project-6/screenshots/1.png)

![truffle test](project-6/screenshots/2.png)

![truffle test](project-6/screenshots/3.png)

![truffle test](project-6/screenshots/4.png)


## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

Please make sure you've already installed ganache-cli, Truffle and enabled MetaMask extension in your browser.

- Contract address [0x67e8464de864d54B72650FD77E54068c6efcba41](https://rinkeby.etherscan.io/address/0x67e8464de864d54B72650FD77E54068c6efcba41)
- Truffle v5.1.14-nodeLTS.0 (core: 5.1.13)
- Solidity v0.5.16 (solc-js)
- Node v12.18.1
- Web3.js v1.2.1
- truffle-hdwallet-provider ^1.0.17
- truffle-assertions ^0.9.2

### Installing

A step by step series of examples that tell you have to get a development env running

Install all requisite npm packages (as listed in ```package.json```):

```
npm install
```
Launch Ganache:

In a separate terminal window, Compile smart contracts:

```
truffle compile
```

Your terminal should look something like this:

![truffle test](project-6/screenshots/compile.png)

This will create the smart contract artifacts in folder ```build\contracts```.

Migrate smart contracts to the locally running blockchain, ganache-cli:

```
truffle migrate --network rinkeby
```

Your terminal should look something like this:

![truffle test](project-6/screenshots/migrate.png)

Test smart contracts:

```
truffle test
```

All 10 tests should pass.

![truffle test](project-6/screenshots/test1.png)

![truffle test](project-6/screenshots/test2.png)

In a separate terminal window, launch the DApp:

```
npm run dev
```
IPFS used:

```
No
```

## UML Diagrams

* [Activity diagram](project-6/screenshots/Activity_UML_Diagram.png?raw=true "Activity diagram")
* [Sequence diagram](project-6/screenshots/Sequence_UML_Diagram.png?raw=true "Sequence diagram")
* [State diagram](project-6/screenshots/State_UML_Diagram.png?raw=true "State diagram")
* [Class diagram](project-6/screenshots/Class_UML.png?raw=true "Class diagram")

## Built With

* [web3.js](https://github.com/ethereum/web3.js/) - web3.js is a collection of libraries which allow you to interact with a local or remote Ethereum node, using an HTTP, WebSocket or IPC connection.
* [Truffle](https://www.trufflesuite.com/docs/truffle/getting-started/installation) - A development environment, testing framework and asset pipeline for blockchains using the Ethereum Virtual Machine (EVM).
* [Infura](https://infura.io) - Provide secure, reliable, and scalable access to Ethereum and IPFS. It also provide the infrastructure for your decentralized applications so you can focus on the features.
* [Metamask](https://metamask.io/) - A bridge that allows you to visit the distributed web of tomorrow in your browser today. It allows you to run Ethereum dApps right in your browser without running a full Ethereum node.

## Acknowledgments

* Solidity
* Ganache-cli
* Truffle
* IPFS
