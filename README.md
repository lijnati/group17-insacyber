#  P2P Communication System (Cybersec + Blockchain + Networking)

## Overview
This project is a **Peer-to-Peer (P2P) Communication System** that enables two clients to communicate directly without routing all traffic through a central server.  
We use:
- **WebRTC** for real-time peer-to-peer connections
- **Blockchain (Ethereum)** for **decentralized identity and peer discovery**
- **A lightweight signaling server** only for exchanging connection info (not for relaying data)

This ensures secure, private, and decentralized communication—ideal for messaging. 

##  Features
✅ Blockchain-based **decentralized peer discovery**  
✅ Wallet-based **identity management** (MetaMask)  
✅ Direct **WebRTC peer-to-peer communication** (data channel)  
✅ **Signaling server** (WebSockets) for offer/answer exchange only  
✅ Real-time **chat messaging** between peers  
✅ Future: **end-to-end encryption (E2EE)** with key exchange  


## Architecture

```mermaid
flowchart TD
    A[Peer 1 (React + MetaMask)] <--WebRTC DataChannel--> B[Peer 2 (React + MetaMask)]
    A <--Offer/Answer/ICE--> S[Signaling Server (WebSocket)]
    B <--Offer/Answer/ICE--> S
    C[Smart Contract (Ethereum)] --> A
    C --> B
```

## 👥 Team

Built at INSA Summer Camp as a collaborative project to explore Cybersecurity + Blockchain + P2P Networking. 
