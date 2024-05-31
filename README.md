# Smart-Contract-Project
This repository is for the project assessment of the project of the 1st module of : solidity-avax-intermediate course of Metacrafters academy . The purpose of creating this to prove my learning and to showcase my skill as a solidity developer to the people.

# Problem Statement
write a smart contract that implements the require(), assert() and revert() statements.

# Description
This program is a simple contract written in Solidity, a programming language used for developing smart contracts on the Ethereum blockchain. The contract has a single function that sets the value of the variable by checking some constrains as given in program to calculate the weight of the object by taking in the mass of the object. As we all know the formulae of i.e. Weight = mass * gravity. This program uses the concept of Functions and Error handling.

It's essential to use these error handling statements judiciously to maintain the security and correctness of your smart contract. Remember that require() and revert() consume all gas when they fail, while assert() should only be used to check for internal errors and should not fail under normal conditions.

# Executing Program
To run this program, you can use Remix, an online Solidity IDE. To get started, go to the Remix website at https://remix.ethereum.org/ .

// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

contract ErrorHandlerContract {
    error InsufficientBalanceError(uint requiredAmount);

    string public tokenName = "MYTOKEN";
    uint256 public totalSupply = 100;
    mapping(address => uint256) public balances;
   
    function customRequireCheck(uint _stock) public pure returns (string memory) {
        uint availableStock = 150;
        require(_stock <= availableStock, "Custom error message: Stocks are not available");
        return "Product is in cart now meanwhile you can proceed further";
    }

 
    function customAssertCondition(uint _value) public pure returns (string memory){
        assert(_value > 0 && _value < 99); 
        return "Custom error message: Value must be between 1 and 99";
}

    function customRevertCondition(uint _balance, uint _amount) public pure {
        if (_balance < _amount) {
            revert("Custom error message: Something went wrong");
        }
    }
}
