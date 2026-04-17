# 🏗️ Architecture

This application is built on the Canopy framework using a plugin-based execution model.

## 🔄 Flow

1. User submits a transaction via Web Wallet
2. Transaction is sent to the node via RPC
3. Node forwards the transaction to the plugin
4. Plugin processes:
   - CheckTx (validation)
   - DeliverTx (execution)
5. Plugin interacts with FSM (state machine)
6. State is updated (balances + fee pool)

---

## ⚙️ Core Components

- Web Wallet (UI)
- RPC Server
- Canopy Node
- Plugin (Go)
- FSM (State Machine)

---

## 🧠 Execution Logic

The core transaction logic lives in:

plugin/go/contract/contract.go

Specifically:
- DeliverTx → executes transfers
- Updates:
  - Sender balance
  - Receiver balance
  - Fee pool

---

## 🔐 Determinism

All state transitions are:
- Deterministic
- Verifiable
- Executed at protocol level

---

## 🚀 Summary

This architecture demonstrates how financial logic can be executed directly at the blockchain protocol layer using Canopy plugins.
