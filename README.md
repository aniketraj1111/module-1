# Project Name: Avalanche-Subnets

## Overview
Welcome to the Avalanche-Subnets project! This guide will walk you through the deployment and testing process for the EVM subnet on Avalanche, along with the deployment of ERC-20 and Vault smart contracts. The ERC-20 contract represents a fungible token, and the Vault contract securely manages the deposit and withdrawal of ERC-20 tokens.

## Process Steps

### 1. Deploy EVM Subnet
Use the Avalanche CLI to deploy your EVM subnet. This step is crucial for setting up the environment for your smart contracts.

### 2. Add Subnet to Metamask
Add your subnet to Metamask and select the network. This ensures seamless integration with your deployed contracts.

### 3. Connect Remix to Metamask
Connect Remix to Metamask using the Injected Provider. This allows you to deploy and interact with your smart contracts directly from Remix.

### 4. Deploy Smart Contracts
Deploy the ERC-20 and Vault smart contracts using Remix. Follow the provided steps in the respective contract sections.

### ERC20 Contract

#### Functions
1. **`transfer`**: Transfer tokens between accounts.
2. **`approve`**: Grant approval for token transfer on behalf of an account.
3. **`transferFrom`**: Transfer tokens from one account to another with approval.
4. **`mint`**: Create and add new tokens to the contract owner's balance.
5. **`burn`**: Burn a specified number of tokens from an account.

#### Events
- **`Transfer`**: Triggered when tokens are transferred.
- **`Approval`**: Triggered when approval for token transfer is granted.

### Vault Contract

#### Constructor
- **`constructor`**: Initialize the contract with the ERC-20 token address.

#### Functions
1. **`deposit`**: Allow users to deposit ERC-20 tokens into the vault, minting corresponding shares.
2. **`withdraw`**: Allow users to withdraw ERC-20 tokens from the vault by burning shares.

#### State Variables
- **`token`**: Address of the ERC-20 token held in the vault.
- **`totalSupply`**: Total number of shares in the vault.
- **`balanceOf`**: Mapping of shares held by each user.

### 5. Test Your Application
After deploying your contracts, thoroughly test your application to ensure proper functionality and security.

## Author
Aniket Raj

Feel free to modify and enhance this readme to make it more attractive and informative for users. 
