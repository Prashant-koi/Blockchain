# Simple Blockchain Implementation

This project demonstrates a basic blockchain implementation written in TypeScript. It includes core blockchain concepts like transactions, blocks, wallets, mining, and digital signatures.

## Features

- **Blockchain Structure**: Implements a chain of blocks linked by cryptographic hashes
- **Digital Signatures**: Uses RSA key pairs to sign and verify transactions
- **Proof of Work**: Simple mining algorithm finding hashes with leading zeros
- **Cryptocurrency**: Basic wallet implementation for transferring funds

## Installation

1. Clone the repository
2. Install dependencies:
   ```bash
   npm install
   ```

## Running the Project

You can run the example blockchain in two ways:

### Option 1: Using the compiled JavaScript
```bash
node index.js
```

### Option 2: Compile and run
```bash
npx tsc
node index.js
```

### Option 3: Add a start script
Add this to your `package.json`:
```json
"scripts": {
  "dev": "tsc --watch",
  "start": "tsc && node index.js"
}
```
Then run:
```bash
npm run start
```

## How It Works

1. **Transactions**: Represent the transfer of funds between wallets
2. **Blocks**: Store transaction data and link to previous blocks via hashes
3. **Chain**: A series of connected blocks forming the ledger
4. **Wallets**: Generate public/private key pairs for secure transactions
5. **Mining**: A proof-of-work system that secures the blockchain

## Example Usage

The example code demonstrates:
- Creating three wallets (satoshi, prasant, jack)
- Executing transactions between them
- Mining new blocks to add these transactions to the chain
- Viewing the blockchain state at the end

## Technical Details

- Written in TypeScript with Node.js
- Uses crypto module for cryptographic operations
- Implements SHA256 for block hashing
- Implements MD5 for proof-of-work mining
- Uses RSA for transaction signing and verification

## Thanks Fireship(Youtube) for teaching!