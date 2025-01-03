SHIPLT

SHIPLT is a shipment tracking system designed to ensure the authenticity of products across the supply chain using Blockchain technology. It involves three key entities: Manufacturer, Seller, and Consumer. The system generates QR codes to verify product details and ensures each stage of the product's journey is tracked.

## Features

1. Manufacturer:
- Add product details.
- Generate a QR code with product details.
- Assign products to sellers via unique seller IDs.

2. Seller:
- List products for sale.
- Sell products to consumers via their unique consumer IDs.
- Track products sold through the system.

3. Consumer:
- Scan the QR code to verify product authenticity (genuine or fake).


## Packages Required

- Truffle v5.6.7 (core: 5.6.7)
- Ganache v7.5.0
- Solidity v0.5.16 (solc-js)
- Node v15.8.0
- Web3.js v1.7.4
- npm 7.5.1

## Other Requirements

- Any Chromium-based browser (e.g., Chrome)
- MetaMask browser extension

## Setup Process

1. **Clone the repository**:
    ```bash
    https://github.com/deepakbaligar-83/SHIPLT.
    ```

2. **Navigate to the project folder and install required dependencies**:
    ```bash
    npm install
    ```

3. **Compile contract source files using Truffle**:
    ```bash
    truffle compile
    ```

4. **Open Ganache and set up a local blockchain**:
    - Create a new workspace
    - Add `truffle-config.js` to your project
    - Change port to `7545` (matching Ganache server settings)

5. **Set up MetaMask**:
    - Open MetaMask in Chrome
    - Add a new test network using:
        - **Network ID**: 5777 (from Ganache settings)
        - **RPC Server**: `HTTP://127.0.0.1:8545` (from Ganache settings)
        - **Chain Code**: 1337
    - Import an account using the private key from Ganache.

6. **Deploy smart contracts**:
    ```bash
    truffle migrate
    ```

7. **Start the development server**:
    ```bash
    npm run dev
    ```

8. **Login to MetaMask and connect the added account to the local blockchain (localhost:3000)**.

9. **Interact with the website to track and verify products**.
