# Project Development Workflow

The **FractionalGoldCoin** smart contract is designed for the Ethereum blockchain to manage a collection of NFTs representing fractional ownership of physical gold coins. This guide outlines how to mint and manage these coins with the integrated functionalities.

## General Information
- **Name:** Fractional Gold Coin 
- **Symbol:** FGC
- **Max Supply:** 5000
- **Standard:** ERC721A
- **GitHub:** [Fractional Gold Coin](https://github.com/GiuBlockchainDEV/Fractional-Gold-Coin)

## Overview of Minting Process and Functionalities

### Minting NFTs
The contract enables the creation of NFTs representing fractional shares of specific gold coins, each uniquely identifiable.

### Batch Minting
Includes a `batchMint` function for minting multiple NFTs in one transaction, streamlining the creation process.

### Fractionalization Structure
- **Representation:** Each NFT represents a fraction of a Britannia Gold coin.
- **Division:** 5,000 fractions each, further divisible into 5 sub-fractions.
- **Pricing:** £1,000 per sub-fraction, £5,000 per full fraction, £25,000,000 for the entire collection.

### Price Evolution
- Initial sale from the Royal Mint to Aureus at £3,600.
- Aureus marks up by 30% (£1,080).
- Post-grading, value increases by 15% (£585) for Grade PF60, with incremental increases for higher grades.

### Staking Mechanism
Owners are required to stake their fractions for 18 months before eligibility for secondary market sales.

### Grading and Value Adjustment
NFT value increases based on coin grading, with preset increments for different grades and additional value for services like vaulting and insurance.

### Metadata Management
Includes detailed off-chain information about each gold coin, linked via a URI.

### Secondary Market Integration
Facilitates NFT trading on secondary markets after the staking period, ensuring contract compatibility with marketplaces.

### Royalty Agreement in Smart Contract
Embeds a royalty agreement directly into the NFT's smart contract, with automatic execution upon secondary sales.

## Key Features

- **ERC721Enumerable:** For better NFT tracking and enumeration.
- **Coin/NFT History Tracking:** Tracks each coin’s history, including price changes and applied services.
- **Dynamic Pricing:** Reflects value changes due to grading and additional services.
- **Chronological Tracing:** Records the stages of each gold coin’s lifecycle.

## Additional Considerations

- **Gas Efficiency:** Optimized for Ethereum’s transaction costs.
- **Security:** Includes robust security measures; auditing recommended.
- **Off-Chain Metadata Storage:** Utilizes IPFS (Pinata Studio) for storing NFT metadata.

## Summary
The FractionalGoldCoin smart contract facilitates the issuance, management, and trading of NFTs tied to physical gold coins, supporting minting large collections, dynamic pricing, and enforcing a staking period.

---

## Development Stages

### 1. Smart Contract Development
- Write initial contract code.
- Implement minting, fractionalization, staking, grading/value adjustment, metadata management, and royalty agreement functionalities.
- Key features: ERC721Enumerable, history tracking, dynamic pricing, and chronological tracing.

### 2. Platform Development
- Develop POC, logo, brand identity, and UI/UX (Figma).
- Front end, server customization, and back end development.
- Conduct rigorous security and functionality testing.

### 3. Secondary Market Integration
- Ensure contract compatibility with NFT marketplaces.
- Implement trading functionality for the post-staking period.

### 4. Additional Considerations
- Optimize for gas efficiency and implement robust security measures.
- Implement off-chain metadata storage and ensure Web3/Web5 compatibility.

### 5. Project Review and Launch
- Final contract code review, security audit, front-end testing, and deployment on the Ethereum network.
- Mint the initial batch of NFTs and launch the project for trading.

## Important Contacts
- **Project Lead:** GiuBlockchainDEV

## Useful Resources
- Ethereum Smart Contract and Solidity Documentation.
- OpenZeppelin Contracts Library, IPFS Documentation, and OpenSea API Documentation.
