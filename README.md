## Foundry

**Foundry is a blazing fast, portable and modular toolkit for Ethereum application development written in Rust.**

Foundry consists of:

-   **Forge**: Ethereum testing framework (like Truffle, Hardhat and DappTools).
-   **Cast**: Swiss army knife for interacting with EVM smart contracts, sending transactions and getting chain data.
-   **Anvil**: Local Ethereum node, akin to Ganache, Hardhat Network.
-   **Chisel**: Fast, utilitarian, and verbose solidity REPL.

## Documentation

https://book.getfoundry.sh/

## Usage

### Build

```shell
$ forge build
```

### Test

```shell
$ forge test
```

### Test Coverage

```
forge coverage
```

and for coverage based testing: 

```
forge coverage --report debug
```

# Audit Scope Details

- Commit Hash:  7d55682ddc4301a7b13ae9413095feffd9924566
- In Scope:
```
./src/
└── PasswordStore.sol
```
- Solc Version: 0.8.18
- Chain(s) to deploy contract to: Ethereum

## Create the audit report

View the [audit-report-templating](https://github.com/Cyfrin/audit-report-templating) repo to install all dependencies. 

```bash
cd audits
pandoc 2023-09-01-password-store-report.md -o report.pdf --from markdown --template=eisvogel --listings
```