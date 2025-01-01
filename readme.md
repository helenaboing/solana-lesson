# Keypair Management

This repository provides scripts for generating and loading keypairs used in Solana development.
This code in this repository was developed using the Solana tutorial "Intro to Cryptography": [Solana Tutorial](https://solana.com/pt/developers/courses/intro-to-solana/intro-to-cryptography)

## Keypair Generation

Use the `keypair-generate.ts` script to generate a new public and private keypair. This is essential for creating secure transactions on the Solana blockchain.

### Usage

1. Run the script:
   ```bash
   ts-node keypair-generate.ts
   ```

2. The output will display the generated public and secret keys:
   ```
   The public key is: <public_key>
   The secret key is: <secret_key>
   ```

## Keypair Loading

Use the `keypair-load.ts` script to load an existing private key from a `.env` file. This is useful for accessing your keypair securely without hardcoding sensitive information.

### Prerequisites

- Ensure you have a `.env` file in your project root with the following format:
  ```
  SECRET_KEY=<your_secret_key>
  ```

### Usage

1. Run the script:
   ```bash
   ts-node keypair-load.ts
   ```

2. The script will load the private key from the environment and allow you to use it in your application.

## Dependencies

This project requires the following dependencies:

- `@solana-developers/helpers`: A helper library for Solana development.
- `@solana/web3.js`: The official Solana JavaScript API.

You can install the dependencies using npm:
   ```bash
   npm install
   ```