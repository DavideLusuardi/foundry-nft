# FoundryNFT

A simple NFT created using Foundry.

## Foundry

Foundry is a blazing fast, portable and modular toolkit for Ethereum application development written in Rust.

Foundry consists of:

-   **Forge**: Ethereum testing framework (like Truffle, Hardhat and DappTools).
-   **Cast**: Swiss army knife for interacting with EVM smart contracts, sending transactions and getting chain data.
-   **Anvil**: Local Ethereum node, akin to Ganache, Hardhat Network.
-   **Chisel**: Fast, utilitarian, and verbose solidity REPL.

### Installing Openzeppelin

```shell
$ forge install Openzeppelin/openzeppelin-contracts --no-commit
```

### Usage

#### Build

```shell
$ forge build
```

#### Test

```shell
$ forge test
```


#### Help

```shell
$ forge --help
$ anvil --help
$ cast --help
```

#### Deploy

Run this script to deploy and verify the NFT contract on sepolia.

```shell
$ forge create --rpc-url https://rpc2.sepolia.org --private-key $PRIVATE_KEY --etherscan-api-key $ETHERSCAN_KEY --verify src/FoundryNFT.sol:FoundryNFT
```