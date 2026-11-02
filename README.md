# Aave Borrowing Experiments with Hardhat

A small Ethereum / DeFi learning project using Hardhat and ethers.js to interact with Aave contracts. The checked-in scripts focus on obtaining WETH and exercising a borrow flow; this repository is not a complete lending protocol implementation.

## Repository contents

- `scripts/getWeth.js` — obtains WETH for the configured development network.
- `scripts/aaveBorrow.js` — script for an Aave borrowing interaction.
- `contracts/interfaces/` — contract interface definitions.
- `hardhat.config.js` — Hardhat network and Solidity configuration.

## Stack

- Solidity / Hardhat
- JavaScript and ethers.js
- Aave Protocol V2 interfaces
- Chainlink contract dependencies
- dotenv for local configuration

## Setup

Requirements: Node.js and npm.

```bash
git clone https://github.com/Sandeep-kumar-IITR/Undercollateralized-lending-borrowing.git
cd Undercollateralized-lending-borrowing
npm install
cp .env.example .env
```

Edit `.env` with RPC endpoints and test-wallet configuration. Never use a wallet that holds real funds for experiments, and never commit a private key.

## Development

The package scripts include:

```bash
npm run lint
npm run lint:fix
npm run format
```

Review `hardhat.config.js` and the scripts before running a transaction. Use a test network and verify the target network, contract addresses, token approvals and transaction parameters.

## Security status

A credential file was previously committed to this repository and has been removed from the current branch. Treat every credential that appeared in the old file as compromised. Rotate RPC/API credentials and move any funds controlled by the exposed wallet to a new wallet. Removing the file from the latest commit does not remove it from Git history.

## Disclaimer

This is an educational experiment, not an audited protocol or financial product. Do not deploy it with real funds.

## Author

Sandeep Kumar
