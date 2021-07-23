# ETHEREUM Developer

This will serve as markdown notes for all we learn about solidity and Ethereum.

Index:

- [**Truffle**](#Truflle)
- [**Solidity**](#Solidity)
- [**Tests**](#Tests)

  
## Truflle

Is a framework to build daps. Creates a folder with the structure needed to create and deploy smart contracts in solidity. Also it creates a truffle-config.js which serves as a configuration file. You can specify here:

- Solidity compiler version 
- etc.

### How to install it

````
npm install truffle --save-dev 
````

### Init a project

````
mkdir project
cd project
npx truffle init
````

This will create a structure such as: 
```
|-contracts (where you put .sol files)
|-migrations ()
|-test (where you put your tests.)
truffle.config.js
```

#### What's migration for?

*Migrations are Javascript files that help you deploy contracts to the Ethereum network. These files are responsible for staging your deployment tasks, and they're written under the assumption that your deployment needs will change over time. As your project evolves, you'll create new migration scripts to further this evolution on the blockchain. A history of previously run migrations is recorded on-chain through a special Migrations contract, detailed below.**

## Solidity

Solidity is the language to develop byte code for EVM (Ethereum Virtual Machine).

### Visibility and Getters

![4ee95d9b.png](:storage/93c76eaa-7cf8-462d-8a8e-ea41f21bc653/4ee95d9b.png)

## Tests

### Open Zeppelin Test Helpers
[Test Helpers - OpenZeppelin Docs](https://docs.openzeppelin.com/test-helpers/0.5/)



