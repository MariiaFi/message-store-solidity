# MessageStore Solidity Contract

This is a simple smart contract written in Solidity that allows storing and updating a message on the Ethereum blockchain.

## Features
- Store a message when the contract is deployed
- Update the message anytime
- Retrieve the current message

## Smart Contract

```solidity
contract MessageStore {
    string private message;

    constructor(string memory initialMessage) {
        message = initialMessage;
    }

    function setMessage(string memory newMessage) public {
        message = newMessage;
    }

    function getMessage() public view returns (string memory) {
        return message;
    }
}
