**Contract Title:**  ERC20Token 
**Description:** This Solidity smart contract implements a basic ERC20 token with additional functionalities such as minting, burning, and allowance management.

totalSupply: Dynamic (increases with minting and decreases with burning)

**Features:-**
Constructor

Initializes the contract owner as the deployer (msg.sender).
Sets the initial total supply to 0.
Minting (mint function)

Allows the contract owner to mint new tokens and assign them to a specified account.
Emits a Transfer event from the zero address to the recipient account.
Transfer (transfer function)

Enables users to transfer tokens to another account.
Checks if the sender has sufficient balance before proceeding.
Emits a Transfer event from the sender to the recipient.
Transfer From (transferFrom function)

Allows a designated spender to transfer tokens on behalf of another account (fromAccount).
Ensures that the spender has been authorized by the fromAccount to transfer the specified amount.
Emits a Transfer event from the fromAccount to the recipient.
Approval (approve function)

Grants permission to a designated spender to withdraw tokens from the caller's account.
Emits an Approval event indicating the amount approved and the spender's address.
Burn (burn function)

Allows any token holder to burn a specific amount of their own tokens, thereby reducing the total supply.
Emits a Transfer event from the token holder to the zero address.
Balance Inquiry (balanceOf function)

Retrieves the token balance of a specified address.
Allowance Inquiry (allowance function)

Retrieves the amount of tokens that an owner has allowed a spender to withdraw.
Usage
To deploy this contract, compile it with Solidity version ^0.8.0 and deploy it to a supported Ethereum network using tools like Remix, Truffle, or Hardhat.

License
This project is licensed under the MIT License
