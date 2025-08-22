 # Ainur's FHEVM Dashboard

**Ainur — developer, researcher, and advocate for privacy-preserving technologies.**  
This project is my customized adaptation of Zama's `fhevm-react-template`, built on version 0.7 of the FHEVM protocol. It demonstrates how encrypted data can be processed and interacted with on-chain using Fully Homomorphic Encryption, while maintaining user privacy and control.

## 🚀 Features

- 🔐 Increment and decrement an encrypted counter
- 🧠 Request decryption via the Decryption Oracle
- 🦊 Seamless integration with MetaMask and Sepolia testnet
- 🧬 Built with FHEVM v0.7 and Homomorphic Complexity Units (HCU)

## 🧭 Setup & Deployment Steps

This project was manually installed and configured using the following steps:

 **Clone the frontend template**  
   Cloned the `alexB/nextjs-react-v7` branch of Zama's [`fhevm-react-template`](https://github.com/zama-ai/fhevm-react-template).

 **Clone the Hardhat backend**  
   From the project root:
   ```bash
   cd ./packages
   git clone https://github.com/zama-ai/fhevm-hardhat-template.git

Install Hardhat dependencies
cd fhevm-hardhat-template
npm install

Set environment variables 
Configured mnemonic for my wallet:
npx hardhat vars set MNEMONIC
npx hardhat vars set ETHERSCAN_API_KEY

Compile and test contracts locally
npm run compile
npm run test

Deploy to Sepolia Testnet
npx hardhat deploy --network sepolia

Verify contract on Etherscan
npx hardhat verify --network sepolia <CONTRACT_ADDRESS>

Run tests on Sepolia
npx hardhat test --network sepolia

Install frontend dependencies 
From the project root:
cd ..
npm install
npm run dev

Launch frontend 
Opened http://localhost:3000 in browser.

Connect MetaMask to Sepolia 
Switched MetaMask to Sepolia testnet and verified interaction with deployed contract.

📁 Project Structure
packages/site/fhevm: Core hooks for interacting with FHEVM smart contracts

packages/site/hooks/useFHECounter.tsx: Example hook for encrypted counter logic

packages/site/hooks/metamask: MetaMask wallet integration hooks

📚 Resources
Zama FHEVM Documentation

Hardhat + MetaMask Setup Guide

@zama-fhe/relayer-sdk

👤 Author & Contact
Ainur — developer, researcher, and enthusiast of privacy-first technologies. 

📬 Email: jeneshka883@gmail.com

💬 Telegram: @AinurSolar

🐦 X (Twitter): @InurSolar91279

🌐 Farcaster: farcaster.xyz/ainur-zk1


Built with ❤️ by Ainur$ZAMA

📖 [Русская версия README](./README.ru.md)



