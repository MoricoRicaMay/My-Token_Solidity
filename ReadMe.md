# MyToken Solidity

The MyToken Solidity contract is designed for creating and managing a custom token on Ethereum.

## Description

It allows minting tokens to specific addresses via the mint function, increasing the total token supply and updating recipient balances. Tokens can also be burned using the burn function, decreasing the total supply and deducting tokens from addresses with sufficient holdings. The contract maintains token names (tokenName) and abbreviations (tokenAbbrv), and uses a mapping (balances) to track token ownership per address.

## Getting Started

### Installing

To execute this code, you can utilize Remix, an online Integrated Development Environment (IDE) for Solidity. Begin by visiting the Remix website at https://remix.ethereum.org/.

Once on the Remix site, initiate a new file by selecting the "+" symbol located in the left-hand sidebar. Save the file with a .sol extension (for instance, myToken.sol). Proceed by copying and pasting the provided code into this newly created file.

### Executing program

To compile the code, navigate to the "Solidity Compiler" tab located in the left-hand sidebar of the Remix IDE. Ensure that the selected "Compiler" version is set to "0.8.25" or another compatible version. Click on the "Compile myToken.sol" button to initiate the compilation process.

After successfully compiling the code, proceed to deploy the contract by accessing the "Deploy & Run Transactions" tab also found in the left-hand sidebar. Choose the "myToken" contract from the dropdown menu, then click on the "Deploy" button.

Upon successful compilation, proceed to the "Deploy & Run Transactions" tab, click "Deploy" to deploy the contract. Once deployed, you can interact with the contract's functions (mint and burn) and view its public variables (tokenName, tokenAbbrv, totalSupply, and balances) directly within Remix IDE. Use the interface to test various scenarios and ensure the contract functions as intended.
```
// SPDX-License-Identifier: MIT
pragma solidity 0.8.25;

contract MyToken {
    string public tokenName = "TokenNiRica";
    string public tokenAbbrv = "TNR";
    uint public totalSupply = 0;

    mapping (address => uint) public balances;

    function mint(address _address, uint _value) public {
        totalSupply += _value;
        balances[_address] += _value;
    }

    function burn(address _address, uint _value) public {
        if (balances[_address] >= _value) {
            totalSupply -= _value;
            balances[_address] -= _value;
        }
    }
}

```

## Authors

Rica May M. Morico


## License

This project is licensed under the [NAME HERE] License - see the LICENSE.md file for details
