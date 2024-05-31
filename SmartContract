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
