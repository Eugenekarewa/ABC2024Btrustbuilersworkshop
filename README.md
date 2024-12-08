# Bitcoin Transaction Builder Workshop

## Overview

This workshop is designed to help you understand and fix the Bitcoin transaction builder code.
Fix and complete the Bitcoin transaction builder to create valid transactions for the Bitcoin network.

## Prerequisites

Before you begin, ensure you have the following installed:

- [Bun (recommended)](https://bun.sh/docs/installation) or [Node.js](https://nodejs.org/en/download/)
- [Git](https://git-scm.com/downloads)

## Setup

## Quick Start

1. Clone the repository:

```bash
git clone <repository-url>
cd <repository-name>
```

2. Install dependencies:

```bash
bun install
```

or

```bash
npm install
```

## Passing the First Stage

The entry point to the workshop is the [main.ts](app/main.ts) file. To pass the first stage, you need to create an empty commit and push it to the remote repository.

```bash
git commit --allow-empty -m "Pass the first stage"
git push
```

## Passing Other Stages

Study the code in the [main.ts](app/main.ts) file and fix the bugs. There are comments in the code that will guide you to the solution. When you are done, create a new commit and push it to the remote repository.

```bash
git commit -am "Pass the stage"
git push
```

You should see the logs for your changes in your terminal.

You can also run the program manually to test your changes.

```bash
chmod +x ./your_program.sh

./your_program.sh
```

## Objectives

- Understand Bitcoin transaction structure.
- Debug and fix the provided code.
- Generate a valid, signed transaction.

## Skill Areas

- **Bitcoin Protocol**: Transaction creation, validation.
- **Debugging**: Fix broken logic.
- **Signing**: Use ECDSA for inputs.

## Goals

1. Analyze and debug the code.
2. Fix input, output, and signature issues.
3. Test and validate the transaction.

## Example Usage

```javascript
import { createTransaction } from './app/main.ts';

const utxos = [
  { txid: 'abcd1234...', vout: 0, value: 500000 }
];
const targetAddress = 'tb1q...';
const amount = 100000;
const privateKey = 'your_private_key_here';

const rawTx = createTransaction(utxos, targetAddress, amount, privateKey);
console.log(rawTx);
```

## Key Fixes Needed

- Correct UTXO referencing.
- Proper output and fee calculation.
- Implement signature generation.
- Correct transaction serialization.

## Outcome

- A valid Bitcoin transaction ready for signet/testnet.

For every bug you fix, you should see the logs for your changes in your terminal when you push to the remote repository or run the program manually.
