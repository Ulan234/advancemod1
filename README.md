# Solidity by Example (SOLBYEX) - ERC20 Token Contract

## Overview

This Solidity contract represents a basic ERC20 token named "Solidity by Example" with the symbol "SOLBYEX." It is designed to showcase the fundamental functionalities of an ERC20 token on the Ethereum blockchain.

## Contract Details

- **Name:** Solidity by Example
- **Symbol:** SOLBYEX
- **Decimals:** 18
- **Total Supply:** Initially set to 0, will be increased through the `mint` function.
- **Events:** 
  - `Transfer`: Triggered when tokens are transferred between addresses.
  - `Approval`: Triggered when an owner approves an address to spend tokens on their behalf.

## Functions

### `transfer`

```solidity
function transfer(address recipient, uint amount) external returns (bool)
```

Transfers `amount` tokens from the sender's account to the `recipient` account.

### `approve`

```solidity
function approve(address spender, uint amount) external returns (bool)
```

Approves the specified `spender` to spend a given `amount` of tokens on behalf of the owner.

### `transferFrom`

```solidity
function transferFrom(address sender, address recipient, uint amount) external returns (bool)
```

Transfers `amount` tokens from the `sender` account to the `recipient` account. The caller must be an approved spender on behalf of the sender.

### `mint`

```solidity
function mint(uint amount) external
```

Mints new tokens and adds them to the sender's balance and the total supply.

### `burn`

```solidity
function burn(uint amount) external
```

Burns a specified `amount` of tokens from the sender's account, reducing both the sender's balance and the total supply.

## Usage

1. Deploy the contract to the Ethereum blockchain.
2. Interact with the contract using the defined functions to transfer, approve, mint, and burn tokens.

## License

This contract is licensed under the [MIT License](https://opensource.org/licenses/MIT).
