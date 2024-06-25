# MyToken Solidity

The MyToken Solidity contract is designed for creating and managing a custom token on Ethereum.

## Description

It allows minting tokens to specific addresses via the mint function, increasing the total token supply and updating recipient balances. Tokens can also be burned using the burn function, decreasing the total supply and deducting tokens from addresses with sufficient holdings. The contract maintains token names (tokenName) and abbreviations (tokenAbbrv), and uses a mapping (balances) to track token ownership per address.

## Getting Started

### Installing

To execute this code, you can utilize Remix, an online Integrated Development Environment (IDE) for Solidity. Begin by visiting the Remix website at https://remix.ethereum.org/.

Once on the Remix site, initiate a new file by selecting the "+" symbol located in the left-hand sidebar. Save the file with a .sol extension (for instance, HelloWorld.sol). Proceed by copying and pasting the provided code into this newly created file.

### Executing program

To compile the code, navigate to the "Solidity Compiler" tab located in the left-hand sidebar of the Remix IDE. Ensure that the selected "Compiler" version is set to "0.8.4" or another compatible version. Click on the "Compile HelloWorld.sol" button to initiate the compilation process.

After successfully compiling the code, proceed to deploy the contract by accessing the "Deploy & Run Transactions" tab also found in the left-hand sidebar. Choose the "HelloWorld" contract from the dropdown menu, then click on the "Deploy" button.

Once the contract deployment is completed, you can interact with it by invoking the sayHello function. Navigate to the "HelloWorld" contract in the left-hand sidebar, locate the "sayHello" function, and click on it. Finally, execute the function by clicking the "transact" button to retrieve the output message "Hello World!".
```
code blocks for commands
```

## Authors

Contributors names and contact info

ex. Dominique Pizzie  
ex. [@DomPizzie](https://twitter.com/dompizzie)


## License

This project is licensed under the [NAME HERE] License - see the LICENSE.md file for details
