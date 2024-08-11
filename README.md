# BlockchainSimulator

## Overview
BlockchainSimulator is a basic implementation of a blockchain in Java. It demonstrates the creation and mining of blocks, handling transactions, and managing wallet balances. The project uses the BouncyCastle library for cryptographic functions and Gson for JSON handling.

## Features
- Genesis Block Creation: Initialize the blockchain with a genesis block.
- Transaction Handling: Add transactions to blocks and mine them.
- Wallet Management: Create wallets, manage balances, and handle fund transfers.
- Blockchain Validation: Verify the integrity and validity of the blockchain.


## Getting Started
### Prerequisites
- Java JDK (1.8 or higher)
- BouncyCastle library (bcprov-jdk15to18-1.78.1.jar)
- Gson library (gson-2.2.2.jar)

# Project Structure
      noobchain/
      ├── noobchain/
      │   ├── Block.java
      │   ├── NoobChain.java
      │   ├── StringUtil.java
      ├── gson-2.2.2.jar
      ├── bcprov-jdk15to18-1.78.1.jar
      └── README.md


# Getting Started
1. Clone the Repository
git clone https://github.com/Arshi81099/noobchain.git
cd noobchain/src

2. Compile the Project
javac -cp gson-2.2.2.jar:bcprov-jdk15to18-1.78.1.jar noobchain/*.java 

3. Run the Project
java -cp .:gson-2.2.2.jar:bcprov-jdk15to18-1.78.1.jar noobchain.NoobChain

4. Expected Output
When you run the project, it will mine three blocks and display the blockchain in JSON format. The output should look something like this:

`Creating and Mining Genesis block... 
Transaction Successfully added to Block
Block Mined!!! : 000704818a16596f477c7c8795197607dbbd6f297ca169d9bbea7adaa62b8225

WalletA's balance is: 100.0

WalletA is Attempting to send funds (40) to WalletB...
Transaction Successfully added to Block
Block Mined!!! : 0003b18f9b607daed34152eacd433dcde47d2afb0cf332007dd3dee02d5ace8d

WalletA's balance is: 60.0
WalletB's balance is: 40.0

WalletA Attempting to send more funds (1000) than it has...
#Not Enough funds to send transaction. Transaction Discarded.
Block Mined!!! : 000cc8531365a2b22fec1dace21a9149f15df347e3252ceeae1075b3902b879e

WalletA's balance is: 60.0
WalletB's balance is: 40.0

WalletB is Attempting to send funds (20) to WalletA...
Transaction Successfully added to Block

WalletA's balance is: 80.0
WalletB's balance is: 20.0
Blockchain is valid`
