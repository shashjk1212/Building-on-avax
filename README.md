# Decor Token

## Overview
The Decor Token contract is a Solidity smart contract that facilitates the creation, management, and transfer of a custom ERC20 token named "Decor Token" (DECOR). This token can be used as a means of exchange and also for redeeming various types of decor items.

## Features
- ERC20 Compliance: The Decor Token contract inherits from the ERC20 standard, enabling it to function like any other ERC20 token.
- Minting: Only the contract owner can mint new tokens and distribute them to designated addresses.
- Burning: Token holders can burn their tokens to reduce the total token supply.
- Transfer: Token holders can transfer tokens to other addresses.
- Redeeming for Decor: Token holders can redeem their tokens for specific types of decor items based on predefined rates.

## Contract Structure
The contract is structured as follows:

- **DecorToken**: This is the main contract that implements the ERC20 token functionalities. It inherits from OpenZeppelin's ERC20 contract.
- **Ownable**: The contract is owned by an address which has special privileges, such as minting tokens and setting item prices.
- **ERC20Burnable**: Inherits functionality to burn tokens.

## Functions
- **setPrices**: Internal function to set the prices of different types of decor items.
- **setItemPrices**: Allows the contract owner to set prices for different types of decor items.
- **mintTokens**: Allows the contract owner to mint new tokens and distribute them to specified addresses.
- **transferTokens**: Allows token holders to transfer tokens to other addresses.
- **burnTokens**: Allows token holders to burn their tokens, reducing the total token supply.
- **redeemForDecor**: Allows token holders to redeem tokens for specific types of decor items based on predefined rates.
- **getBalance**: Returns the token balance of the caller.
- **determineRedeemedDecor**: Internal function to determine which type of decor item can be redeemed based on the token amount provided.
- **getRecentlyRedeemedDecor**: Returns the most recently redeemed type of decor item.

## Testing
- The contract should be thoroughly tested on a testnet before deploying it to the mainnet to ensure its proper functionality and security.

## MIT License 
Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction.

## Author
shashank jk

shashjk5@gmail.com
