
---

# DeSwap Protocol Interface using uniswap 

DeSwap is an open-source frontend interface for a decentralized exchange protocol. This project provides all the necessary components to interact with a decentralized liquidity protocol, allowing users to swap tokens, add or remove liquidity to pools, and manage their positions.

This interface is a fork of the original Uniswap V2 interface, providing a robust and well-tested foundation for decentralized trading.

## Features

-   **↔️ Token Swaps:** Seamlessly swap between a wide variety of ERC20 tokens. The interface automatically finds the best trading routes for optimal prices.
-   **💧 Liquidity Pools:** Add your tokens to liquidity pools to earn trading fees or remove your liquidity at any time.
-   **📈 V1 & V2 Support:** Includes functionality to interact with both V1 and V2 liquidity pools, along with tools to migrate V1 liquidity to V2.
-   **🔍 Token Lists:** Supports community-curated token lists to easily find and import desired tokens, minimizing the risk of interacting with malicious contracts.
-   **🌐 Wallet Integration:** Connects with a variety of wallets like MetaMask, WalletConnect, Coinbase Wallet, Fortmatic, and Portis using Web3-React.
-   **⚙️ Advanced Controls:** For experienced users, "Expert Mode" allows for higher slippage tolerance and custom transaction deadlines.
-   **📊 Transaction Management:** View your recent transaction history and track their status directly within the interface.
-   **🌍 i18n Support:** Includes localization for multiple languages.

---

## 🛠️ Technology Stack

-   **Frontend:** React, TypeScript, Redux & Redux Toolkit
-   **Blockchain SDK:** Uniswap V2 SDK (`@uniswap/sdk`)
-   **Wallet Connectivity:** Ethers.js, Web3-React
--   **Styling:** Styled Components
-   **Development/Build:** Create React App, Yarn, Prettier, ESLint
-   **Testing:** Cypress (Integration), Jest (Unit)

---

## 🚀 Getting Started

To get a local copy up and running, follow these steps.

### Prerequisites

-   [Node.js](https://nodejs.org/) (`>=10.0.0`)
-   [Yarn](https://yarnpkg.com/)
-   [Git](https://git-scm.com/)
-   A Web3 wallet extension in your browser (e.g., MetaMask) configured for a testnet like Sepolia.

### Installation & Setup

1.  **Clone the repository:**
    ```sh
    git clone https://github.com/Pradise2/deswap.git
    ```
2.  **Navigate into the interface directory:**
    ```sh
    cd deswap/interface
    ```
3.  **Install dependencies:**
    ```sh
    yarn install
    ```
4.  **Run the development server:**
    ```sh
    yarn start
    ```

The application should now be running locally at `http://localhost:3000`.

### Configuring the Environment (Optional)

To have the interface default to a different network when a wallet is not connected:

1.  In the `interface` directory, make a copy of `.env.production` and name it `.env.local`.
2.  Change `REACT_APP_CHAIN_ID` to your desired network ID (e.g., `"11155111"` for Sepolia).
3.  Change `REACT_APP_NETWORK_URL` to your RPC endpoint (e.g., `"https://sepolia.infura.io/v3/YOUR_INFURA_KEY"`).

---

## 📂 Project Structure

The repository is structured as a monorepo containing two main packages:

-   `interface/`: The React-based frontend application that users interact with.
-   `v2sdk/`: The core SDK for programmatic interaction with the Uniswap V2 protocol smart contracts.

---

## 🤝 Contributing

This project is based on the original Uniswap V2 interface. Contributions that improve functionality, fix bugs, or enhance the user experience are welcome.

1.  Fork the Project
2.  Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3.  Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4.  Push to the Branch (`git push origin feature/AmazingFeature`)
5.  Open a Pull Request

---

## 📜 License

This project is licensed under the **GNU General Public License v3.0**. See the `LICENSE` file for more details.
