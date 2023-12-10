# ChocolateContract

## Overview

ChocolateContract is a Solidity smart contract that facilitates the purchase and consumption of virtual chocolates. It allows users to buy chocolates and the contract owner to consume them.

## Features

- **Purchase Chocolate**: Users can buy chocolates by calling the `purchaseChocolate` function, specifying the quantity they want to purchase.
- **Consume Chocolate**: The contract owner can consume chocolates using the `consumeChocolate` function, limiting consumption to one unit at a time.

## Getting Started

### Prerequisites

- Ethereum wallet or compatible browser extension (e.g., MetaMask)
- Access to an Ethereum testnet or mainnet for deployment and interaction

### Deployment

1. Deploy the `ChocolateContract` to an Ethereum network using Solidity compiler version ^0.8.0.
2. Specify an owner for the contract during deployment.

### Interacting with the Contract

#### `purchaseChocolate(uint256 sum)`

- **Parameters**:
  - `sum`: The quantity of chocolates to purchase.
- **Usage**:
  - Users can call this function, sending ETH equivalent to the cost of chocolates (`sum` * 1). The purchased chocolates will be added to the sender's stock.

#### `consumeChocolate(uint256 quantity)`

- **Parameters**:
  - `quantity`: The quantity of chocolates to consume.
- **Usage**:
  - Only the contract owner can call this function. They can consume chocolates from their stock, limited to one unit per call.

## Notes

- Ensure proper handling of Ether sent with function calls to prevent loss of funds.
- Use appropriate precautions when interacting with Ethereum contracts on live networks.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## Author

Hemanth N

hemeee1111@gmail.com
