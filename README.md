# ♻️ Stellar Atomic Swap

A simple implementation of **Atomic Swap** on the Stellar blockchain — enabling two parties to securely and simultaneously exchange assets **without intermediaries**.

---

## 💡 What is an Atomic Swap?

An **Atomic Swap** is a type of smart transaction that ensures:

- Either **both parties successfully exchange assets**, or
- **Nothing happens at all**

This avoids the risk of one party sending assets and the other failing to reciprocate.

---

## ⚙️ How It Works

This implementation uses **pre-signed transactions** and **multisig logic** on Stellar:

- Party A locks XLM/token to be released only if Party B signs
- Party B signs a matching transaction
- When both sides are satisfied and time conditions are met, the transactions are submitted

All or nothing.

---
## 🛠️ Setup Instructions

1. Clone the repository and install dependencies:

```bash
git clone https://github.com/yourusername/atomic-swap.git
cd atomic-swap
npm install
