# 🌾 AgriChain: Revolutionizing Agriculture with Decentralized Technology

[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![GitHub stars](https://img.shields.io/github/stars/YourUsername/AgriChain?style=social)](https://github.com/YourUsername/AgriChain/stargazers)
[![Built with React](https://img.shields.io/badge/Frontend-React.js-blue)](https://reactjs.org/)
[![Smart Contracts](https://img.shields.io/badge/Blockchain-Solidity%20%7C%20Ethereum-orange)](https://ethereum.org/en/developers/docs/)
[![AI Powered](https://img.shields.io/badge/AI%20Insights-Gemini%20API-yellow)](https://ai.google.dev/)

## 🌟 Project Overview

**AgriChain** is a decentralized web application (dApp) built to solve core inefficiencies in the traditional agricultural supply chain. By leveraging **Ethereum Smart Contracts**, **IPFS decentralized storage**, and cutting-edge **AI insights**, we connect farmers directly with consumers and laborers, ensuring transparency, security, and profitability.

This project was initially developed as a Mini-Project at SJEC

## ✨ Key Features

AgriChain is built on three core modules, enhanced by AI:

| Module | Description | Core Technology |
| :--- | :--- | :--- |
| **Direct Marketplace** | [cite_start]Allows farmers to list and sell produce directly to consumers, cutting out intermediaries and increasing farmer profit margins[cite: 71, 111]. | Ethereum Smart Contracts |
| **Labor Hiring Platform** | [cite_start]Streamlines the process for farmers to post job listings and for agricultural laborers to find work[cite: 96, 113]. | Smart Contracts |
| **Information Hub** | [cite_start]Provides a platform for sharing agricultural news, best practices, and innovations[cite: 97, 143]. | IPFS Decentralized Storage |
| **AI Decision Engine** | **Smart Pricing** (real-time market analysis) and **Crop Prediction** (best to grow advice) powered by the **Gemini API** for strategic guidance. | Gemini API (AI Insights) |

## ⚙️ Technical Stack

This project employs a robust, full-stack decentralized architecture:

| Component | Technology | Role |
| :--- | :--- | :--- |
| **Blockchain** | **Ethereum** | Hosts and executes critical transactions. |
| **Smart Contracts** | **Solidity** (v0.8.20+) | Logic for product sales, labor contracts, and user roles. |
| **Development Tools** | **Truffle Suite, Ganache** | Contract testing, debugging, and local blockchain environment. |
| **Frontend** | **React.js, Tailwind CSS** | [cite_start]User interface, wallet connection, and application state management[cite: 178]. |
| **Blockchain Interaction** | **Web3.js, MetaMask** | [cite_start]Connects the React frontend to the Ethereum network[cite: 176]. |
| **Decentralized Storage** | **IPFS** | [cite_start]Securely stores non-transactional data like product images and articles[cite: 177, 416]. |
| **Backend (Off-Chain)** | **Node.js** (for IPFS/SMS bridge) | [cite_start]Handles off-chain communication and API requests[cite: 179]. |

## 🚀 Getting Started

Follow these steps to set up and run the AgriChain dApp locally.

### Prerequisites

1.  **Node.js** (v18+) and npm/yarn
2.  **Ganache** Desktop Application (for a local blockchain)
3.  **MetaMask** Browser Extension

### 1. Blockchain Deployment (The Decentralized Backend)

Navigate to the `agrichain-blockchain/` directory.

1.  **Install Truffle (Global)**:
    ```bash
    npm install -g truffle
    ```
2.  **Start Ganache**: Open the Ganache application and note the RPC URL (`http://127.0.0.1:7545`) and Network ID (`5777`).
3.  **Compile & Migrate Contracts**:
    ```bash
    cd agrichain-blockchain
    truffle migrate --network development
    ```
    *Note the deployed **Contract Address** from the output; you will need to add this to the frontend configuration.*

### 2. Frontend Setup (The React dApp)

Navigate to the `agrichain-frontend/` directory.

1.  **Install Dependencies**:
    ```bash
    cd ../agrichain-frontend
    npm install
    ```
2.  **Configure API Keys & Contract Address**:
    Create a `.env` file and add your credentials and the deployed contract address:
    ```
    # Replace with your actual deployed address
    REACT_APP_CONTRACT_ADDRESS=0x...
    
    # Required for AI features (Pricing, Crop Prediction)
    REACT_APP_GEMINI_API_KEY=YOUR_GEMINI_API_KEY_HERE 
    ```
3.  **Run the Application**:
    ```bash
    npm start
    ```
    The application will open at `http://localhost:3000`.

### 3. Connect Wallet

1.  Open MetaMask and add a **Custom Network** pointing to your Ganache RPC URL (`http://127.0.0.1:7545`).
2.  Import an account (using a private key from Ganache) to use as a testing wallet (Farmer/Consumer).

## 🤝 Contribution

Contributions are welcome! Please follow these steps:

1.  Fork the repository.
2.  Create a feature branch (`git checkout -b feature/AmazingFeature`).
3.  Commit your changes (`git commit -m 'Add some AmazingFeature'`).
4.  Push to the branch (`git push origin feature/AmazingFeature`).
5.  Open a Pull Request.

## 👥 Project Team

* **Titus Dias S**
* **Nithin **
* **Hemant Murlapur**
* **Thilask**



## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.

---
[cite_start]*AgriChain is a step toward modernizing agriculture through decentralized technology, with the potential to improve efficiency, transparency, and profitability in the sector.* [cite: 53]
