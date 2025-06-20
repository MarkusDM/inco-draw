# IncoDraw ♠ — Fully Onchain Card Game on Inco

**IncoDraw** is a fully on-chain, encrypted PvP card game built on the **Inco** blockchain.  
Inspired by the classic Eastern European card game "Durak", IncoDraw brings high-stakes card battles and private gameplay into a trustless Web3 format.

Players create or join rooms, stake tokens, and play with encrypted decks — all actions are verifiable yet confidential. The winner takes the pot.

---

## 🎮 Game Overview

- Players **create** or **join** a room
- The creator sets a **wager** (INCO tokens)
- Cards are **encrypted and dealt on-chain**
- Players take turns attacking and defending
- The player who discards all cards first **wins the pot**

---

## 🧾 Game Rules (Inspired by Durak)

### 🎴 Setup

- **2 players**, PvP format
- **36-card deck** (6 to Ace) across 4 suits
- A **trump suit** is randomly selected at game start
- Each player is dealt **6 encrypted cards**
- First attacker is randomly chosen

### ▶️ Turn Flow

#### 1. Attack Phase
- Attacker plays **1 card**
- Defender must beat it with:
  - A higher card of the **same suit**, or
  - **Any trump** card

#### 2. Defense & Add-ons
- If defender successfully defends, attacker may **add more cards** matching the existing ranks
- Defender must beat all cards (max 6 cards per turn)

#### 3. Outcome
- ❌ If defense fails → defender **takes all cards**
- ✅ If defense succeeds → cards go to **discard pile**

#### 4. Refill
- Players **draw encrypted cards from the deck** until they each have 6 (if possible)
- Turn passes:
  - If defender succeeded → they become attacker
  - Otherwise → attacker continues

#### 🏆 Win Condition
- First player to get rid of all cards **wins**
- Last player holding cards is the **loser**

---

## 📊 Deck Structure

- Total: **36 cards**
- Suits: ♠ Spades, ♥ Hearts, ♦ Diamonds, ♣ Clubs
- Ranks: 6, 7, 8, 9, 10, J, Q, K, A
- One random **trump suit**
- Cards are encrypted using **Inco Confidential Tokens** — visible only to the holder

---

## 🔄 UX Flow

### For Player A (Creator):
1. Connect wallet (Inco-compatible)
2. Set **stake amount**
3. Click **Create Room**
4. Wait for opponent to join

### For Player B (Joiner):
1. Connect wallet
2. Join open room
3. Confirm & lock stake

### During Game:
- Game logic is managed via smart contracts
- Cards are encrypted → only visible to the owner
- Players interact via frontend UI (play, defend, draw)
- All state changes are **on-chain and verifiable**

### End:
- Winner automatically receives **wagered pot**
- Game is archived on-chain with full state proof

---

## 🔐 Why Inco?

- Zero-knowledge–powered **Confidential Token SDK**
- Fully encrypted game state
- 100% on-chain logic, no servers
- Private, fair, and decentralized gameplay

---

## ⚙️ Tech Stack

- [Inco Confidential Token SDK](https://docs.inco.org/tutorials/confidential-token)
- [Inco Solidity SDK](https://docs.inco.org/solidity-sdk)
- [Inco JS Client SDK](https://docs.inco.org/js-sdk/client-sdk)
- Frontend: React or Svelte
- Wallet support: Inco Snap / MetaMask
- Smart contracts:
  - Game room & staking
  - Encrypted card dealing
  - Turn logic and outcome validation

---

## 🧠 Roadmap

- [ ] Define full game logic (onchain + encrypted)
- [ ] Implement confidential card system
- [ ] Smart contracts for room creation, staking, payouts
- [ ] MVP frontend with wallet integration
- [ ] Internal testing & testnet launch
- [ ] Public mainnet release

---

## 💡 About the Name

**IncoDraw** blends "drawing cards" and "strategic duels" in a privacy-first, trustless game.  
Powered by the Inco blockchain.

---

Made with ♥️ on [Inco](https://docs.inco.org/)

