# 🚀 JERUZZALEM Canopy Transfer App

Built with Canopy Go Plugin Template • Demonstrates protocol-level transaction execution

## 🧠 One-line Pitch

A minimal reference implementation of protocol-level transaction execution using Canopy plugins, demonstrating deterministic state transitions and onchain fee accounting.

---

## 📌 Overview

Canopy is a modular blockchain framework that allows custom transaction execution via plugins at the protocol level.

This app is built using the Canopy Go Plugin Template.

It demonstrates a working onchain transaction system where:

* Users can send tokens
* Balances are updated onchain
* Fees are collected into a fee pool
* Custom plugin logic is executed during transactions

This project focuses on execution at the protocol layer rather than the smart contract layer.

---

## ⚙️ Features

* Onchain token transfer
* Balance updates
* Fee pool system
* Custom DeliverTx execution
* Real-time plugin logging

---

## 🧪 How It Works

1. User sends transaction via Web Wallet
2. Transaction enters mempool
3. Plugin validates (CheckTx)
4. Plugin executes (DeliverTx)
5. State updates:

   * Sender balance decreases
   * Receiver balance increases
   * Fee pool increases

---

### 🔄 Execution Flow

```text
[Wallet]
   ↓
[RPC]
   ↓
[Node]
   ↓
[Plugin]
   ↓
[FSM / State]
```
---

## 🎥 Demo Video

Live execution demo (local environment, showing real transaction flow and state updates):

https://x.com/0XJERUZZALEM_/status/2045100818152693934 (thread)

https://x.com/0XJERUZZALEM_/status/2045107184405782714 (thread)

https://x.com/0XJERUZZALEM_/status/2045118301236547798

---

## 📸 Proof (Execution Log)

```
🚀 TX EXECUTED FROM PLUGIN
StateWrite SUCCESS!
```

---

## 📂 Code Structure

* plugin/go/contract/contract.go → core transaction execution logic (CheckTx & DeliverTx)

---

## 🚀 Status

✔ Running locally
✔ Transactions successful
✔ Plugin modified and verified

---

## 💡 Why This Matters

Most Web3 apps operate at the smart contract layer.

This project demonstrates how financial logic can be executed directly at the protocol layer using Canopy plugins.

This enables:
- Lower-level control over transaction execution
- Deterministic and verifiable state transitions
- Custom fee mechanisms beyond standard smart contracts

## 🧬 What Makes This Different

Unlike typical smart contract-based systems, this app:

- Executes logic at the protocol level (not EVM / contract layer)
- Hooks directly into CheckTx and DeliverTx lifecycle
- Controls state transitions via plugin-based execution

## 🔮 Future Use Cases

- Decentralized payment system
- Onchain treasury tracking
- Automated fee distribution engine

---

## ▶️ How to Run

```bash
git clone https://github.com/EdLWEISS186/JERUZZALEM-canopy-transfer-app.git
cd JERUZZALEM-canopy-transfer-app
canopy start
```
Then open:

- Web Wallet: http://localhost:50000
- Explorer: http://localhost:50001

---

This project serves as a minimal reference for building custom execution logic directly at the blockchain protocol layer using Canopy.
