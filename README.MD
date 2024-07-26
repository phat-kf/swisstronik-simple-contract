# Swisstronik Testnet Task: Deploy a simple contract using Hardhat

This repository contains the necessary scripts to set up and interact with a smart contract on the Swisstronik Testnet using Hardhat.

## Install Dependency:

NodeJS >= v22.0.4

## Setup Instructions

1. **Clone the Repository:**
```sh
git clone https://github.com/dante4rt/swisstronik-testnet.git
cd swisstronik-testnet
```

2. **Run the Setup Script:**
```sh
./swisstronik.sh
```

3. **Follow the Prompts:**
    * Choose JavaScript when prompted.
    * Use the default directory (just press Enter).
    * Press y to confirm any prompts.

4. **Copy your Contract address**
    ...
    Swisstronik contract deployed to `###`
    ...
5. **Upload your .sol contract file**
    * Create a repository in github
    * Create a new file and name it: `Hello_swtr.sol`
    * paste following code in it and save it
    ```sh
    // SPDX-License-Identifier: UNLICENSED
    pragma solidity ^0.8.19;

    contract Swisstronik {
        string private message;

    constructor(string memory _message) payable {
        message = _message;
    }

    function setMessage(string memory _message) public {
        message = _message;
    }

    function getMessage() public view returns(string memory) {
        return message;
    }
    ```

## Complete task: Deploy a simple contract using Hardhat

Submit your `Hello_swtr.sol github url` + `contract address`

[https://www.swisstronik.com/testnet2/dashboard#](https://www.swisstronik.com/testnet2/dashboard#)