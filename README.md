# Base on Mars NFT Project

Base on Mars is a unique NFT collection that spans across two blockchains - Ethereum and Solana - connected via LayerZero's cross-chain messaging protocol.

## Overview

The project consists of two complementary NFT contracts:
- An ERC-721 contract deployed on Ethereum
- An SPL Token contract deployed on Solana

These contracts work together to create a seamless cross-chain NFT experience where actions on one chain can trigger effects on the other through LayerZero's messaging layer.

## Architecture

The system uses LayerZero's cross-chain messaging to maintain state consistency between the two NFT collections. When certain actions occur on one chain (like minting or burning), corresponding updates are triggered on the other chain through LayerZero's messaging protocol.

### Ethereum Contract
- Standard ERC-721 implementation
- Integration with LayerZero's endpoint for cross-chain messaging
- Ability to trigger state changes on the Solana side

### Solana Contract  
- SPL Token implementation
- Integration with LayerZero's Solana endpoint
- Capability to receive and process messages from the Ethereum contract

## Cross-Chain Functionality

The NFTs on both chains are linked through LayerZero, enabling:
- Cross-chain ownership verification
- Synchronized minting/burning across chains
- Unified metadata and attributes
- Seamless transfer of NFT properties between chains

## Technical Details

The project leverages:
- Foundry for Ethereum development (see below for Foundry-specific commands)
- Anchor framework for Solana development
- LayerZero's messaging protocol for cross-chain communication
