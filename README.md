# MyToken Solidity Contract

## Overview
This is a basic Solidity smart contract named `MyToken` that implements a simple token with minting and burning functionalities. The contract allows for creating (minting) and destroying (burning) tokens, while keeping track of balances and the total token supply.

## Contract Details
- **Token Name:** Vishwas
- **Token Abbreviation:** Vish
- **Initial Total Supply:** 0

## Features
1. **Public Variables**
   - `myTokenName`: Stores the name of the token.
   - `myTokenAbbrv`: Stores the abbreviation of the token.
   - `totalSupply`: Stores the total number of tokens minted.

2. **Mapping**
   - `balance`: Maps addresses to their respective token balances.

3. **Functions**
   - `mint(address _address, uint _value)`: Allows minting new tokens. Increases the total supply and the balance of the specified address by `_value`.
   
   - `burn(address _address, uint _value)`: Allows burning (destroying) tokens. Decreases the total supply and the balance of the specified address by `_value`, if the address has sufficient tokens to burn.

## Usage
1. **Deployment**
   - Deploy the contract on a supported Ethereum Virtual Machine (EVM) using a development environment like Remix.

2. **Interacting with the Contract**
   - Use the `mint` function to create new tokens.
   - Use the `burn` function to destroy tokens.

3. **Considerations**
   - Ensure that the address calling the `burn` function has enough tokens to burn, as the function includes a check to prevent burning more tokens than owned.
