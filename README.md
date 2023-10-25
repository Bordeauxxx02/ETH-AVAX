# Error Handling Smart Contract

This is a Solidity smart contract demonstrating error handling mechanisms.

## Smart Contract Details

- **Contract Name**: `errorHandling`
- **Solidity Version**: ^0.8.0

### Functions

1. `deposit(uint amount)`
   - Allows users to deposit Ether into their account.
   - Requirements: Amount must be greater than 0.

2. `transfer(address to, uint value)`
   - Allows users to transfer Ether to another address.
   - Requirements:
     - User must have sufficient balance.
     - Destination address must be valid.
     - Checks for potential overflow.

3. `withdraw(uint value)`
   - Allows users to withdraw Ether from their account.
   - Requirements: User must have sufficient balance.

4. `sendEtherWithRevert(address to, uint value)`
   - Demonstrates an intentional revert scenario.
   - Requirements:
     - User must have sufficient balance.
     - Destination address must be valid.
     - Checks for potential overflow.
   - Triggers a revert with the message "Intentional revert".

### Events

- `Deposit(address indexed from, uint value)`
- `Transfer(address indexed to, uint value)`
- `Withdraw(address indexed to, uint value)`
- `SentEther(address indexed from, address indexed to, uint value)`
