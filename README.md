# Fibonacci.sol
Fibonacci.sol
pragma solidity ^0.8.20;
contract Fibonacci {
    function fib(uint n) public pure returns(uint) {
        if(n <= 1) return n;
        uint a = 0;
        uint b = 1;
        for(uint i=2;i<=n;i++){
            uint c = a + b;
            a = b;
            b = c;
        }
        return b;
    }
}
