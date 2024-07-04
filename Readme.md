
# MyToken

## Definition
**MyToken** is a custom Solidity ERC-20-like token. It can mint and burn tokens, while using public variables to store the name, abbreviation, and total supply of the token. This contract has a mapping for addresses with their balances of tokens.

## Requirements

### Public Variables:
- **tokenName**: The name of the token.
- **tokenAbbrv**: The abbreviation of the token.
- **totalSupply**: Token’s total supply.

### Mapping:
- **balances**: Stores addresses as well as their respective balances on tokens.

### Mint Function:
- Takes an address and a value as parameters.
- Increases the total supply by that value.
- Increases the balance of the specified address by the same amount.

### Burn Function:
- Takes an address and a value as parameters.
- Ensures that the specified amount isn’t greater than or equal to the balance at the specified address to be burnt.
- Reduces total supply by this amount.
- Reduces the balance at the specified address by the same volume.

## Execution Process

### Prerequisites
- Ensure you have Node.js and npm installed.
- Install Truffle or Hardhat for contract deployment and testing.
- Set up a local Ethereum blockchain using Ganache or use a testnet like Rinkeby.

## Installation
1. Clone the repository:
    ```bash
    git clone https://github.com/EthereumProofAssesment/MyToken.git
    ```
2. Navigate to the project directory:
    ```bash
    cd MyToken
    ```
3. Install the dependencies:
    ```bash
    npm install
    ```

## Usage
### Compile the Contract
```bash
truffle compile
