# Smart-Contract-Project
This repository is for the project assessment of the project of the 1st module of : solidity-avax-intermediate course of Metacrafters academy . The purpose of creating this to prove my learning and to showcase my skill as a solidity developer to the people.

# Problem Statement
write a smart contract that implements the require(), assert() and revert() statements.

# Description
This program is a simple contract written in Solidity, a programming language used for developing smart contracts on the Ethereum blockchain. The contract has a single function that sets the value of the variable by checking some constrains as given in program to calculate the weight of the object by taking in the mass of the object. As we all know the formulae of i.e. Weight = mass * gravity. This program uses the concept of Functions and Error handling.

It's essential to use these error handling statements judiciously to maintain the security and correctness of your smart contract. Remember that require() and revert() consume all gas when they fail, while assert() should only be used to check for internal errors and should not fail under normal conditions.

# Executing Program
To run this program, you can use Remix, an online Solidity IDE. To get started, go to the Remix website at https://gitpod.io/#https://github.com/jeffryan-POL/solidity_starter.

Once you are on the Remix website, create a new file by clicking on the "+" icon in the left-hand sidebar. Save the file with a .sol extension (e.g., playground.sol). Copy and paste the following code written by me into the file.

To compile the code, click on the "Solidity Compiler" tab in the left-hand sidebar. Make sure the "Compiler" option is set heigher to "0.8.1" (or another compatible version), and then click on the "Compile playground.sol" button.

Once the code is compiled, you can deploy the contract by clicking on the "Deploy & Run Transactions" tab in the left-hand sidebar. Select the "SmartContract" contract from the dropdown menu, and then click on the "Deploy" button.

Once the contract is deployed, you can interact with it by calling the Weight function to set the value, to perform the multiplication and value variable check to check the value of the variable that is publick so we can check that. Finally, click on the "transact" button to execute the function and retrieve the values and messages
