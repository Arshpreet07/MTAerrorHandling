# Error Handling in solidity 

## Description

This Solidity program is a simple program that demonstrates the use of assert(),require() and revert() functions.

## Getting Started

### Executing program

To run this program, you can use Remix, an online Solidity IDE. To get started, go to the Remix website at https://remix.ethereum.org/.

Once you are on the Remix website, create a new file by clicking on the "+" icon in the left-hand sidebar. Save the file with a .sol extension (e.g., HelloWorld.sol). Copy and paste the following code into the file:

// SPDX-License-Identifier: MIT
pragma solidity 0.8.18;

contract ErrorHandling{
    function Requires(uint age) public pure{
        require(age>=18,"Age should be more than 18!");
    }
    function Asserts(uint age) public pure{
        assert(age>=18);
    }
    function reverts(uint age) public pure{
        if(age<18){
            revert("Age should be more than 18");
        }
    }
}

## Authors

Arshpreet Singh
@arshpreet07
