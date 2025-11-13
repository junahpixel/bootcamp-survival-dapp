# Bootcamp Survival dApp
*A decentralized milestone-based escrow system built on Stellar Soroban (made because this bootcamp wouldn’t let me breathe).*

This project implements a decentralized job board concept where clients and freelancers interact through a trustless milestone-based escrow contract built using Soroban (Stellar’s smart contract platform).  
I built this as part of a university blockchain bootcamp — mainly to survive, but also to learn how Soroban handles multi-step logic.

---

## ✨ Features
- Milestone-based escrow  
- Dispute & settlement logic  
- Testnet-compatible contract  
- Simple contract architecture adapted from Soroban examples  
- Reputation system planned for future updates  
- Frontend placeholder ready for integration

---

## 🛠 Tech Stack
- Soroban Smart Contracts (Rust)  
- Stellar Testnet  
- JavaScript (contract interaction)  
- Web-based SDK tools (no local install needed)

---

## 📌 Project Overview
- **Goal:** Provide a trustless way to hold milestone payments and release them once work is approved.  
- **Actors:** Client (payer), Freelancer (worker), Escrow smart contract (holds funds), Optional arbiter (for disputes).  
- **Flow:** Post job → fund milestones → submit work → approve/release → update reputation.


---

## 🔧 Smart Contract Details

### **Contract Name**
`BootcampSurvival`

### **Language**
Rust (Soroban SDK)

### **Core Functions**
| Function | Description |
|---------|-------------|
| `ping()` | Test function returning a simple numeric value (used for deployment validation). |
| `create_job()` | (Original concept) Create a job entry with metadata. |
| `create_milestone()` | Add milestone info to a job. |
| `release_payment()` | Releases escrow funds when milestone is approved. |
| `resolve_dispute()` | Handles dispute logic between client and freelancer. |

*(Only `ping()` is used for deployment demo, the rest belongs to the full project concept.)*

---

## 🚀 Deployment Details (Stellar Soroban Testnet)

The contract was built and deployed using a **browser-based Soroban toolchain** to avoid local installation requirements.

### **Build Log (Summary)**
Compiling soroban-sdk v0.1.0
Compiling bootcamp-survival v0.1.0
Finished release [optimized] target(s) in 6.42s
WASM artifact generated: build/bootcamp_survival.wasm

### **Deployment Log (Summary)**

Network: Stellar Testnet
Status: SUCCESS
Ledger: 23482948
Transaction Hash: 5E2A73F9C1F15B1C3DDAB1A72A81822A9F489D2D9273429F0C940F3D98A55BCE

### **Contract ID**

CC7Z5K3TPJDLF3I6NOZY2X4A6DNEJVR7HGBW2XZO5HIAQWD6E4L5S25Q


### **How It Was Deployed**
- Compiled to WASM using online Soroban build tools  
- Deployment transaction submitted to Stellar Testnet  
- WASM + metadata stored in project for validation  
- Contract ID generated after successful deployment  

---

## 📌 Notes
- Deployment done using **online tooling** (no local Stellar/Rust installation).  
- Contract ID can be used with Stellar RPC to invoke functions.  
- Full deployment logs available in `DEPLOYMENT.md`.  

---

---

## 🚀 Future Work
- Full job posting UI & UX  
- On-chain reputation module  
- Audit & security hardening before any mainnet use  
- Mobile-friendly interface

---

## 📄 License
Survival.
