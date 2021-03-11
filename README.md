//Ethereum_Faucet.sol

pragma solidity ^0.4.19;

contract Faucet{
    
    function Withdraw(uint withdrawAmt) public {
        
        //limt the ether withdrawal
        require(withdrawAmt <=100);
        
        
        //send amount to the adress requested
        msg.sender.transfer(withdrawAmt);
        
        //accept ether
      function () public payable {}
        
    }
    
    
    
}
