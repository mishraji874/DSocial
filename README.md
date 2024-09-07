# DSocial: Decentralized Social Media DApp with Hardhat, React, and TailwindCSS

## Overview

This project demonstrates how to build a decentralized social media dApp using Hardhat for smart contract development, React for the frontend, and TailwindCSS for styling. The dApp leverages blockchain technology to ensure the authenticity and immutability of user posts.

## Prerequisites

* Node.js and npm (or yarn) installed
* A Metamask wallet or similar Ethereum wallet
* An Ethereum network provider (e.g., Infura, Alchemy)

## Demo: [DSocial Website](https://dsocial-pi.vercel.app/)
## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/mishraji874/DSocial.git
   ```

2. Navigate to the project directory:
   ```bash
   cd DSocial
   ```

3. Install dependencies:
   ```bash
   yarn
   ```

4. Install all the dependencies in the client folder:
   ```bash
   yarn
   ```

## Setting Up Environment Variables

1. Create a `.env` file at the root of the project.
2. Add your Ethereum network provider URL and other necessary environment variables:
   ```
    RPC_URL=<YOUR-SEPOLIA-RPC-URL>
    PRIVATE_KEY=<YOUR-PRIVATE-KEY>
    ETHERSCAN_API_KEY=<YOUR-ETHERSCAN-API-KEY>
   ```

## Running the Project
1. Deploy the contract on the Sepolia Chain:
   ```bash
   npx hardhat ignition deploy ./ignition/modules/deploy.js --network sepolia
   ```

2. Start the development server:
   ```bash
   cd client
   yarn start
   ```
   The dApp will be accessible at http://localhost:3000.

## How it Works

1. **Smart Contract:** The smart contract deployed on the blockchain handles user registration, post creation, and interactions (likes, comments).
2. **Frontend (React):** The React frontend interacts with the smart contract using Ethers.js to create and manage user accounts, post content, and view the feed.
3. **Data Storage:** User data and post content can be stored on-chain or off-chain (e.g., IPFS) depending on your requirements.
4. **TailwindCSS:** Provides a utility-first CSS framework for styling the user interface.

## Additional Notes

* Customize the frontend and backend to suit your specific requirements.
* Consider implementing additional features like user profiles, private messaging, or content moderation.
* Ensure proper error handling and user experience throughout the application.