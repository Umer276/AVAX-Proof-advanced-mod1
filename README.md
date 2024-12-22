Prerequisites

    Golang: Install Golang to build avalanche-cli.
    Node.js: Required for running the local Avalanche node.
    Avalanche CLI: Follow the Avalanche CLI installation guide.
    MetaMask: Set up MetaMask and configure it to connect to your local Avalanche node.
    Remix: Open Remix IDE and create a new workspace for managing smart contracts.

1. Set Up Local Avalanche Subnet
Create a Subnet Configuration

    Run the command:

    avalanche subnet create

    Follow the wizard prompts:
        Name: Choose a name for your Subnet (e.g., mySubnet).
        VM: Select SubnetEVM as the Virtual Machine.
        ChainID: Choose a ChainID (e.g., 43113).
        Configure additional options as needed.

Deploy the Subnet

    Export the Subnet configuration:

avalanche subnet export

Deploy the Subnet locally:

    avalanche subnet deploy --local

2. Deploy Smart Contracts
Compile the Contracts

    Open Remix IDE and import your contract files:
        token.sol
        vault.sol
    Compile both contracts using Remix's compiler.

Connect to the Local Node

    In Remix, navigate to the Deploy tab.
    Under Environment, select Injected Web3.
    Ensure MetaMask is connected to the local Avalanche node.

Deploy the Contracts

    In the Remix Deployer section, select the contract to deploy.
    Provide constructor arguments if needed.
    Click Deploy and confirm the transaction in MetaMask.

3. Interact with Contracts

    Use Remix to:
        Call functions in the contracts.
        Read and write data.
        Monitor events and transactions.

This process enables you to set up a local Avalanche Subnet and deploy smart contracts for development and testing purposes. Let me know if you need further assistance!
