# FundManager Smart Contract

## Overview

The `FundManager` contract is designed for managing a balance, allowing users to deposit, withdraw, and check the current balance.

## Functions

### `deposit(uint256 amt)`

Allows users to deposit a specified amount into the contract's balance.

- **Parameters:**
  - `amt`: The amount to be deposited.

- **Conditions:**
  - The deposit amount must be greater than zero.

- **Implementation:**
  - Increases the contract's balance by the specified amount.
  - Utilizes `require` to ensure the deposit amount is greater than zero.
  - Employs `assert` to verify the correctness of the balance update.

### `withdraw(uint256 amt)`

Allows users to withdraw a specified amount from the contract's balance.

- **Parameters:**
  - `amt`: The amount to be withdrawn.

- **Conditions:**
  - The withdrawal amount should be greater than zero and less than the current balance.

- **Implementation:**
  - Decreases the contract's balance by the specified amount.
  - Checks if the withdrawal amount is valid; otherwise, reverts with an error message.
  - Utilizes `assert` to verify the correctness of the balance update.

### `showBalance()`

Returns the current balance of the contract.

- **Returns:**
  - `uint256`: The current balance.

