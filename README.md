# Simple Royalty Distribution System

## 📌 Project Title
**Simple Royalty Distribution System**

## 📄 Project Description
A decentralized royalty contract designed to manage and distribute earnings fairly among multiple stakeholders (e.g., artists, producers, contributors) based on predefined percentages.

## 🌟 Project Vision
To eliminate disputes and ensure fair, transparent, and automated royalty distribution directly on-chain.

## ✨ Key Features
- Register royalty splits per content ID
- Automatically calculate payouts based on incoming revenue
- Basis point accuracy (supports fractional revenue splits)
- Transparent, tamper-proof distribution records

## 📜 Contract Details

### Contract Address: CDYHRGGDDNSP4LDOJ67SDBQS6MSOAHEXBBSFA33PUSXXCQPZ3UPJH4ZD

### `set_royalties(env, content_id, stakeholders)`
Registers stakeholders and their revenue shares (must total 100%).

- `content_id`: A unique symbol representing the content (e.g., song, book, video)
- `stakeholders`: A list of recipients with their respective percentages in basis points

### `distribute(env, content_id, amount) -> Map<Address, u64>`
Returns the payout map for all stakeholders based on the given revenue amount.

---

Built using the [Soroban SDK](https://soroban.stellar.org/) for fast, secure and gas-efficient smart contracts on the Stellar blockchain.
