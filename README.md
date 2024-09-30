# Lottery Smart Contract

This `Lottery` smart contract allows users to participate in a decentralized lottery on the Ethereum blockchain. The contract's owner can start and end the lottery, and users can buy tickets for a fixed price (10 ETH). At the end of the lottery, a random winner is selected, and 90% of the funds are transferred to the winner, while 10% are transferred to a charity (represented by the owner in this example).

## Features

- **Start a Lottery**: The contract owner can start a new lottery round.
- **Buy Lottery Tickets**: Participants can buy tickets by sending 10 ETH per ticket.
- **Select a Winner**: The contract owner selects a winner at random and distributes the prize.
- **Charity Donation**: 10% of the total funds are donated to a charity (contract owner in this case).
- **Lottery Reset**: Once a winner is selected, the lottery is reset for the next round.

## Requirements

- The contract is deployed on the Ethereum blockchain.
- Participants must send exactly 10 ETH to buy a ticket.
- Only the owner of the contract can start the lottery and select the winner.

## Functions

### 1. `startLottery()`

```solidity
function startLottery() public onlyOwner
