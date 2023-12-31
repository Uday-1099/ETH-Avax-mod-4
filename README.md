## ETH-Avax-mod-4

# MyToken Smart Contract (DegenToken)

This repository contains the Solidity smart contract for the custom ERC20 token named "DegenToken" (symbol: "DGN"). The contract is built on the Ethereum blockchain and follows the ERC20 standard, making it compatible with various decentralized applications (dApps), wallets, and exchanges that support ERC20 tokens.

# Overview

The MyToken.sol file in this repository contains the source code for the DegenToken smart contract. It extends the standard ERC20 contract provided by the OpenZeppelin library and includes additional functionalities for token minting, burning, and transfers. The contract also implements an ownership mechanism, allowing the contract owner to perform certain privileged actions.

# Features

ERC20 Compliance: DegenToken is an ERC20-compliant token, enabling it to be used seamlessly with other ERC20-compatible platforms and services.

Token Minting: The contract owner can create new DegenToken tokens by calling the mint function, allowing for controlled and responsible token issuance.

Token Burning: Token holders can burn their tokens using the burn function. This action is irreversible and effectively reduces the total supply of DegenToken.

Token Redemption: Users can redeem (burn) their DegenToken tokens through the redeem function, reducing their balance by the specified amount.

Redemption for Confectionery Store Items: The contract owner offers a confectionery store where users can redeem their tokens for specific items. The available items are as follows:

Item 1: Candy (Cost: 75 DGN)
Item 2: Cake (Cost: 50 DGN)
Item 3: Doughnut (Cost: 25 DGN)

Transfer and Approvals: Token holders can transfer tokens to other addresses using the standard transfer function. Additionally, they can authorize specific addresses (spenders) to transfer tokens on their behalf using the approve and transferFrom functions.

# Getting Started

Ensure you have the required development environment:

Solidity compiler version 0.8.0 or higher.
Truffle (optional but recommended for testing and deployment).
Install the necessary dependencies:

npm install @openzeppelin/contracts (to fetch the OpenZeppelin library)
Compile the contract:

Run solc MyToken.sol to compile the contract.
Deploy the contract:

Deploy the compiled contract to the Ethereum blockchain using tools like Remix or Truffle.
Usage

To deploy the MyToken contract and create the DegenToken:

Ensure you have the necessary Solidity compiler and development environment set up.

Import the required libraries:

hardhat/console.sol: For logging messages during contract execution.
@openzeppelin/contracts/token/ERC20/ERC20.sol: For implementing the ERC20 token standard.
@openzeppelin/contracts/access/Ownable.sol: For managing contract ownership.
Deploy the contract by providing the desired constructor parameters (name and symbol).

As the contract owner, you can mint new tokens using the mint function.

Token holders can transfer and burn their tokens using transfer and burn functions.

Users can redeem tokens for confectionery store items using the redeemTokens function, specifying the item number they wish to purchase (1 for Candy, 2 for Cake, and 3 for Doughnut).

# Security Considerations

Carefully manage the contract ownership and ensure only trusted parties can access the minting functionality.

Be cautious when transferring token ownership to avoid potential security risks.

Always review and audit the code before deploying to a live network, as smart contract interactions are irreversible.

# License

This smart contract is released under the MIT License. See the LICENSE file for more details.

# Disclaimer

This smart contract is provided as-is and may not have been audited for security or suitability for specific use cases. Use it at your own risk, and always perform thorough testing and security assessments before deploying to a production environment. The contract's developers and contributors are not liable for any damages or losses incurred from its use.
