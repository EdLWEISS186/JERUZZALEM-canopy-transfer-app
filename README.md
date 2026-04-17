# 🚀 JERUZZALEM Canopy Transfer App

Built with Canopy Go Plugin Template • Demonstrates protocol-level transaction execution

## 🧠 One-line Pitch

A simple onchain transfer system built on Canopy that demonstrates real-time balance updates, fee handling, and custom plugin execution.

---

## 📌 Overview

This app is built using the Canopy Go Plugin Template.

It demonstrates a working onchain transaction system where:

* Users can send tokens
* Balances are updated onchain
* Fees are collected into a fee pool
* Custom plugin logic is executed during transactions

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

## 🎥 Demo Video

Here's some proof

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

* plugin/go/contract/contract.go → main logic

---

## 🚀 Status

✔ Running locally
✔ Transactions successful
✔ Plugin modified and verified

---

## 💡 Why This Matters

This app demonstrates how financial logic can be fully executed onchain, including:
- Transparent fee accounting
- Deterministic state updates
- Verifiable transaction execution

It can be extended into:
- DeFi systems
- Payment rails
- Onchain accounting tools

## 🔮 Future Use Cases

- Decentralized payment system
- Onchain treasury tracking
- Automated fee distribution engine
