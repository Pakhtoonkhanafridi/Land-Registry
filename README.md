Land Registry System
A blockchain-based land ownership management system built on Ethereum using Solidity smart contracts. This decentralized application provides a transparent and secure way to manage property transfers with proper verification processes.

🏗️ Project Structure
text
Land-Registry/
├── contracts/
│   └── LandOwnership.sol  # Main smart contract
├── scripts/               # Deployment scripts
├── tests/                 # Test files
└── README.md
📋 Prerequisites
Basic understanding of Ethereum and smart contracts

Remix IDE (online at remix.ethereum.org)

MetaMask wallet browser extension

Test ETH (for test networks like Goerli or Sepolia)

🚀 Getting Started in Remix
Open Remix IDE: Navigate to remix.ethereum.org

Create a new file:

Click on the "File Explorer" icon in the left sidebar

Click the "Create new file" button

Name the file LandOwnership.sol

Copy the contract code:

Paste the provided Solidity code into the new file

Save the file (Ctrl+S)

Compile the contract:

Click on the "Solidity compiler" icon in the left sidebar

Select the appropriate compiler version (0.8.0 or higher)

Click "Compile LandOwnership.sol"

Deploy the contract:

Click on the "Deploy & run transactions" icon

Select "Injected Provider - MetaMask" as the environment

Make sure your MetaMask is connected to a test network

Enter the required constructor parameters:

_landDescription: A description of the land

_seller: The seller's Ethereum address

Click "Transact" and confirm the transaction in MetaMask

🧩 Contract Functions
Role Management
registerInspector(): Register a new land inspector

registerBuyer(): Register as a property buyer

registerSeller(): Register as a property seller

Property Management
registerLand(): Add a new property to the registry

verifyLand(): Land inspector verifies a property

rejectLand(): Land inspector rejects a property

Verification Functions
verifySeller(): Verify a seller's identity

verifyBuyer(): Verify a buyer's identity

Ownership Transfer
transferLandOwnership(): Transfer property to a new owner

Query Functions
checkLandOwner(): Check if address owns a specific property

getLandPrice(): Get the price of a property

getArea(): Get the area of a property

Various verification status checks

🧪 Testing
To test the contract in Remix:

Switch to the "JavaScript VM" environment in the deployment tab

Deploy the contract with test parameters

Use the deployed contract functions to test various scenarios:

Register different roles (inspector, seller, buyer)

Add a property

Verify the property and participants

Simulate ownership transfer

🌐 Deployment to Testnet
Ensure you have test ETH in your MetaMask wallet

Select "Injected Provider - MetaMask" in Remix

Choose a test network (Goerli, Sepolia, etc.) in MetaMask

Deploy the contract as described above

Note the contract address after deployment

🔐 Security Considerations
Always test on a testnet before deploying to mainnet

Carefully review all access control modifiers

Ensure proper verification flows are followed

Consider adding additional security measures for production use

📝 License
This project is licensed under the GPL-3.0 License - see the SPDX identifier in the contract code for details.

🤝 Contributing
Fork the repository

Create a feature branch

Make your changes

Add tests for new functionality

Submit a pull request

⚠️ Important Notes
This is a demonstration contract and should be thoroughly audited before use in production

Real estate regulations vary by jurisdiction - ensure compliance with local laws

Consider adding additional features like escrow payments for production use
