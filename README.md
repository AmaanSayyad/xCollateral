# xCollateral

xCollateral is an overcollateralized DeFi platform built on the XRP Ledger (XRPL) with support for EVM-compatible side chains, leveraging XRPL's native AMM for fast token swaps, bridging, and secure cross-chain lending. The platform offers a transparent, secure, and lightning-fast DeFi solution where users can lend tokens, borrow stable coins, and earn interest through a system that automatically monitors and liquidates under-collateralized loans.

![working-flow](https://github.com/user-attachments/assets/0ee0f691-0707-4b3d-b8ea-25705f91ee47)

## Features
- **Overcollateralized Loans**: Borrowers provide collateral worth more than the loan, minimizing risk for lenders.
- **AMM-Powered Liquidation**: XRPL’s AMM enables rapid liquidation of collateral for stable coins if a loan becomes under-collateralized.
- **Stable Coin Bridging**: Transfers stable coins from XRPL to EVM-compatible side chains.
- **Transparent Oracles**: The witness server provides real-time price data, ensuring secure, transparent monitoring and liquidation of loans.
- **Auto-Rewards**: Incentivizes both lenders and borrowers with rewards based on platform activity.

## Technology Stack
- **XRPL**: Provides the core ledger and AMM functionality.
- **EVM-Compatible Side Chains**: Enhances platform scalability and functionality using Solidity-based smart contracts.
- **Witness Server**: Tracks price data for secure monitoring and immediate liquidation of under-collateralized loans.
- **Frontend**: Built with React for a user-friendly interface.
- **Backend**: Golang and `xrpl.js` for XRPL interactions, wallet creation, token minting, and bridging.

### Prerequisites
- Node.js and npm
- Golang
- XRPL SDK (`xrpl.js`)
- Docker (optional, for local development)

## Usage
**Loan and Lending Process:**
1. **Deposit Collateral:** Users deposit collateral to access overcollateralized loans.
2. **Borrow Stable Coins:** After providing collateral, users can borrow stable coins bridged to EVM side chains.
3. **Automatic Liquidation:** If a loan becomes under-collateralized, the platform automatically liquidates collateral using XRPL’s AMM.
4. **Earn Interest:** Lenders earn interest on their tokens provided to the platform.

**Monitoring and Liquidation:**

The witness server constantly monitors the collateral and loan status. If a borrower’s collateral falls below the required threshold, the system automatically liquidates a portion of the collateral to stabilize the loan.

## Future Improvements
- **Improving Bridge Security:** Developing more robust security features for the bridging process between XRPL and EVM side chains.
- **Enhanced Documentation:** Comprehensive guides for witness server setup and bridge configuration.
- **Expanding Cross-Chain Compatibility:** Supporting additional blockchains for broader platform accessibility.
