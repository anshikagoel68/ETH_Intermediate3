**Contract Name:**  ERC20Token 
**License:** This contract is licensed under the MIT License.
**Compliation Version:** This contract is compile with Solidity version ^0.8.0 and deployed using  Remix IDE.

**Description:** This Solidity smart contract implements a basic ERC20 token with additional functionalities such as minting, burning, and allowance management.

**Contract Details:-**
(a) totalSupply: Dynamically tracks the total supply of tokens issued (increases with minting and decreases with burning).
(b) balances: Mapping of addresses to their respective token balance.
(c) allowed: Nested mapping to track allowances granted for transferring tokens on behalf of others.

**Features:-**
1) Constructor
~ Initializes the contract owner as the deployer (msg.sender).
~ Sets the initial total supply to 0.

2) Minting(mint function)
~ Allows the contract owner to mint new tokens and assign them to a specified account.
~ Emits a Transfer event from the zero address to the recipient account.

3) Transfer(transfer function)
~ Enables users to transfer tokens to another account.
~ Checks if the sender has sufficient balance before proceeding.
~ Emits a Transfer event from the sender to the recipient.

4) Transfer From(transferFrom function)
~ Allows a designated spender to transfer tokens on behalf of another account (fromAccount).
~ Ensures that the spender has been authorized by the fromAccount to transfer the specified amount.
~ Emits a Transfer event from the fromAccount to the recipient.

5) Burn(burn function)
~ Allows any token holder to burn a specific amount of their own tokens, thereby reducing the total supply.
~ Emits a Transfer event from the token holder to the zero address.

6) Balance Inquiry(balanceOf function)
~ Retrieves the token balance of a specified address.



