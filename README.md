# Celo NFT MINTER
This repository contains a simple React Dapp for minting nft on Celo blockchain.

## 1. Tech Stack
This boilerplate uses the following tech stack:
- [React](https://reactjs.org/) - A JavaScript library for building user interfaces.
- [use-Contractkit](contractkit
) - A frontend library for interacting with the Celo blockchain.
- [Hardhat](https://hardhat.org/) - A tool for writing and deploying smart contracts.
- [Bootstrap](https://getbootstrap.com/) - A CSS framework that provides responsive, mobile-first layouts.

## 2. Quick Start

To get this project up running locally, follow these simple steps:

### 2.1 Clone the repository:

```bash
git clone https://github.com/dacadeorg/celo-react-boilerplate.git
```

### 2.2 Navigate to the directory:

```bash
cd celo-react-boilerplate
```

### 2.3 Install the dependencies:

```bash
npm install
```

### 2.4 Run the dapp:

```bash
npm start
```

To properly test the dapp you will need to have a Celo wallet with testnet tokens.
This learning module [NFT Contract Development with Hardhat](https://hackmd.io/exuZTH2hTqKytn2vxgDmcg) will walk you through the process of creating a Metamask wallet and claiming Alfajores testnet tokens.

The boilerplate should behave like this:
![](https://raw.githubusercontent.com/dacadeorg/celo-development-201/main/content/gifs/boilerplate_demo.gif)

## 3. Smart-Contract Deployment

### 3.1 Compile the smart contract

```bash
npx hardhat compile
```

### 3.2 Run tests on smart contract

```bash
npx hardhat test
```

### 3.3 Update env file

- Create a file in the root directory called ".env"
- Create a key called MNEMONIC and paste in your mnemonic key. e.g

```js
MNEMONIC = "...";
```

In this case, we are using a mnemonic from an account created on Celo Extension Wallet. You can copy it from your Celo Wallet account settings.

### 3.4 Deploy the smart contract to the Celo testnet Aljafores

```bash
npx hardhat run --network alfajores scripts/deploy.js
```

This command will update the src/contract files with the deployed smart contract ABI and contract address.