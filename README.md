# ERC-20 Token Contract

Simple ERC-20 token contract written in Solidity.

## 📝 Description

This Solidity contract defines a basic ERC-20 token with standard functions for token transfer, balance checking, and allowance management.

## 🚀 Features

- Name: ERC20Token
- Symbol: Customizable
- Decimals: 18
- Total Supply: Customizable
- Transfer: Implemented
- Approve: Implemented
- Transfer From: Implemented

## 🛠️ Usage

1. Deploy the contract to a compatible Ethereum blockchain.
2. Initialize the contract with parameters: name, symbol, decimals, and initial supply.
3. Interact with the contract using supported functions:
   - `transfer`: Transfer tokens to another address.
   - `approve`: Approve an address to spend tokens on behalf of the owner.
   - `transferFrom`: Transfer tokens from one address to another, with approval.
   - `balanceOf`: Check the balance of a specific address.
   - `allowance`: Check the amount of tokens an owner allowed to a spender.

## 📜 Example

```solidity
// Deploy contract
const myToken = await ERC20Token.deploy("MyToken", "MTK", 18, 1000000);

// Transfer tokens
await myToken.transfer(toAddress, 100);

// Approve spender
await myToken.approve(spenderAddress, 50);

// Transfer from approved tokens
await myToken.transferFrom(ownerAddress, toAddress, 50);
