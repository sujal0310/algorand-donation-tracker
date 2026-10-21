# Algo Fund

A transparent, decentralized crowdfunding platform built on the Algorand blockchain.

![Algorand](https://img.shields.io/badge/Blockchain-Algorand-black)
![Status](https://img.shields.io/badge/Status-In%20Development-orange)
![License](https://img.shields.io/badge/License-MIT-blue)

## Overview

Algo Fund lets creators launch fundraising campaigns and lets backers contribute ALGO directly through smart contracts. Funds are held on-chain and released only when the campaign rules are met, so no middleman controls the money.

## Problem Statement

Traditional crowdfunding platforms have several issues:

- High platform fees (often 5-10% of funds raised)
- Lack of transparency in how funds are held and spent
- Centralized control: the platform can freeze campaigns or funds
- Slow payouts and refunds when a campaign fails

## Proposed Solution

Algo Fund uses Algorand smart contracts to:

- Hold contributions in escrow until the campaign ends
- Release funds to the creator only if the funding goal is reached before the deadline
- Automatically refund backers if the goal is not met
- Make every contribution publicly verifiable on the blockchain

Algorand's low transaction fees and fast finality make small contributions practical.

## Key Features

- **Create campaigns:** set a title, funding goal and deadline
- **Contribute:** back any active campaign with ALGO
- **Escrow:** funds are locked in the smart contract during the campaign
- **Goal-based release:** the creator withdraws funds only if the goal is met
- **Automatic refunds:** backers reclaim funds if the campaign fails
- **Transparency:** public view of total raised, backers and transactions

## How It Works

1. A creator deploys a campaign with a goal amount and deadline.
2. Backers send ALGO to the campaign's smart contract.
3. The contract tracks each contribution and the total raised.
4. After the deadline:
   - **Goal met:** the creator withdraws the funds.
   - **Goal not met:** each backer can claim a refund.

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Blockchain | Algorand (TestNet) |
| Smart contracts | Algorand Python (algopy) / PyTeal |
| Tooling | AlgoKit |
| Wallet | Pera Wallet / Lute (planned) |
| Frontend | React (planned) |
| Version control | Git and GitHub |

## Project Structure

```
algo-fund/
├── contracts/      # Smart contract source code
├── tests/          # Contract tests
├── frontend/       # Web interface (planned)
├── docs/           # Design notes and diagrams
├── README.md
├── LICENSE
└── .gitignore
```

## Getting Started

> Setup steps will be completed as development progresses.

### Prerequisites

- Python 3.12+
- [AlgoKit](https://github.com/algorandfoundation/algokit-cli)
- Git

### Installation

```bash
git clone https://github.com/<your-username>/algo-fund.git
cd algo-fund
algokit bootstrap all
```

## Roadmap

- [x] Create repository and project structure
- [ ] Design smart contract logic
- [ ] Implement campaign creation and contribution
- [ ] Implement withdrawal and refund logic
- [ ] Write tests
- [ ] Build frontend
- [ ] Deploy to Algorand TestNet


## Author

Sujal Khatri
