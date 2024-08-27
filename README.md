# MyCustomToken Smart Contract

## Overview

This Solidity smart contract represents a simple ERC20-like token implementation called `MyCustomToken`. It includes basic functionality for token management, such as minting and burning tokens. The contract tracks token details such as the token name, symbol, and total supply. It also maintains user balances and allows for token supply adjustments.

## Contract Details

### Token Details

- **Token Name**: CryptoGalaxy
- **Token Symbol**: CG
- **Total Token Supply**: Managed internally by the contract

### Functions

1. **`addTokens(address recipient, uint amount)`**

   - **Description**: Mints new tokens and assigns them to a specified address. Increases the total token supply.
   - **Parameters**:
     - `recipient`: The address to receive the new tokens.
     - `amount`: The number of tokens to mint.
   - **Usage**: 
     ```solidity
     addTokens(address recipient, uint amount);
     ```

2. **`removeTokens(address account, uint amount)`**

   - **Description**: Burns tokens from a specified address, decreasing the total token supply.
   - **Parameters**:
     - `account`: The address from which tokens will be burned.
     - `amount`: The number of tokens to burn.
   - **Usage**: 
     ```solidity
     removeTokens(address account, uint amount);
     ```
   - **Requirements**: The account must have a balance greater than or equal to the amount to be burned.

## Installation

To use this contract, you need to have the Solidity compiler installed. You can compile and deploy this contract using tools such as [Remix IDE](https://remix.ethereum.org), [Truffle](https://www.trufflesuite.com/), or [Hardhat](https://hardhat.org/).

### Example with Remix IDE

1. Go to [Remix IDE](https://remix.ethereum.org).
2. Create a new file and paste the contract code.
3. Compile the contract using the Solidity compiler.
4. Deploy the contract to a local or test Ethereum network.

## Usage

After deploying the contract, you can interact with it by calling the `addTokens` and `removeTokens` functions from your Ethereum wallet or through a web3 interface.

- To **mint tokens**, call the `addTokens` function with the recipient's address and the number of tokens.
- To **burn tokens**, call the `removeTokens` function with the account's address and the number of tokens to remove.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request with any improvements or bug fixes.

## Contact

For any questions or feedback, please contact [your email] or open an issue in the repository.

---

Happy coding!

