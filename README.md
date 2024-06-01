# Simple Blockchain Implementation

This repository contains an implementation of a simple blockchain using Python. The code demonstrates the basic principles of blockchain technology, including block creation, hashing, and chain validation.

## Prerequisites

- Python 3.x
- hashlib library (standard in Python)

## Setup

To set up the development environment, ensure you have Python 3.x installed. No additional libraries are required as `hashlib` is part of the Python standard library.

## Implementation Details

### Block Structure

Each block in the blockchain is represented by the `Block` class. A block contains the following attributes:
- `index`: The position of the block within the blockchain.
- `timestamp`: The time at which the block was created.
- `data`: The data contained within the block.
- `previous_hash`: The hash of the previous block in the chain.
- `hash`: The hash of the current block, generated from its content.

### Generating Hashes

The `Block` class includes a method to generate a SHA-256 hash of the block's content. This ensures the integrity and immutability of the data within the block.

### Blockchain Initialization

The `Blockchain` class initializes the blockchain with a genesis block, which is the first block in the chain. The genesis block is created with predefined data and a predefined hash.

### Adding Blocks

The `Blockchain` class includes a method to add new blocks to the chain. Each new block must contain the hash of the previous block to maintain the integrity of the chain.

### Validation

The blockchain can be tested by adding new blocks and verifying the integrity of the chain.

## Usage

1. Clone the repository.
2. Run the Python script to see the blockchain in action.
