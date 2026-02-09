# blockchain-learning
# Blockchain Learning Journey This repository documents my journey into blockchain and smart contracts as an MSc Financial Technology student at the University of Glasgow.

#First Smart Contract
This is the first contract I built for this project.
The idea is simple.
It’s just a basic digital wallet on Ethereum.
You can deposit ETH.
You can withdraw ETH.
And you can only touch your own money.
That’s it.
I built this contract to make sure I properly understood the core Solidity ideas before moving on to anything more complex like time locks.
Here’s how it works in practice:
If you send ETH to the contract, it gets recorded under your address.
When you withdraw, the contract checks your balance first.
If you try to withdraw more than you have, the transaction fails.
One user can never withdraw another user’s funds.
Under the hood, this contract helped me learn a few important things:
How mapping is used to track balances for each address
How msg.sender identifies who is interacting with the contract
How payable functions receive ETH
How require is used to stop invalid actions before they cause problems
This contract isn’t meant to be fancy or production-ready.
Its only purpose is to prove that the basics work and that I understand them.
