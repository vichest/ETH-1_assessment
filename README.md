# ETH-1_assessment
# MyToken Contract

This repository contains a Solidity smart contract for the implementation of a token called "BEAUTY" (abbrv. "BTY"). The contract includes functionalities for minting and burning tokens, as well as maintaining balances and total supply.

## Requirements

1. The contract has public variables to store the details about the token, including its name, abbreviation, and total supply.
2. It utilizes a mapping to associate addresses with token balances (`address => uint`).
3. The contract includes a `mint` function that takes an address and a value as parameters. This function increases the total supply by the given value and increments the balance of the sender's address accordingly.
4. Additionally, the contract includes a `burn` function that works opposite to the `mint` function. It accepts an address and a value as parameters, deducts the value from the total supply, and decreases the sender's balance accordingly.
5. The `burn` function includes conditionals to ensure that the balance of the sender is greater than or equal to the amount intended to be burned.

## Usage

To utilize this contract, follow the steps below:

1. Clone the repository: `git clone https://github.com/your-username/your-repo.git`
2. Navigate to the project directory: `cd your-repo`
3. Compile the Solidity contract using a suitable Solidity compiler (e.g., [solc](https://solidity.readthedocs.io/en/latest/installing-solidity.html)). For example, using solc: `solc --version` to verify the installation and `solc --bin --abi MyToken.sol -o ./bin` to compile the contract.
4. Deploy the compiled contract using a suitable Ethereum development framework (e.g., [Hardhat](https://hardhat.org/), [Truffle](https://www.trufflesuite.com/truffle)). Refer to the framework's documentation for detailed deployment instructions.
5. Interact with the deployed contract by invoking its functions, such as `mint` and `burn`, passing the required parameters.

## License

This code is released under the MIT License. See [LICENSE](./LICENSE) for more information.
