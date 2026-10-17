---
title: Kraken: connect with an API key
date: 2026-10-16
summary: Create a read-only key on Kraken, plus a separate Kraken Futures key if you trade futures. Takes five minutes.
order: 3
kind: guide
---
With an API key Kryptokompis fetches everything from Kraken by itself: trades, deposits and withdrawals, staking and Earn, and futures. The key can only read - Kryptokompis can never trade or withdraw.

## 1. Create the spot key
1. Log in to Kraken (Kraken Pro in the browser).
2. Open the profile menu top right → **Settings** → **API** (may be called *Connections & API*).
3. Choose **Create API key** and name it, e.g. "Kryptokompis".
4. Tick **only** these permissions:
    - **Query Funds**
    - **Query Open Orders & Trades** and **Query Closed Orders & Trades**
    - **Query Ledger Entries**
5. Leave everything called *Deposit*, *Withdraw*, *Create & Modify Orders* and *Cancel/Close Orders* off.
6. Press **Generate key**. Copy the **API key** and **Private key** right away - the private key is shown only once.

## 2. Futures (only if you trade futures)
Kraken Futures has its own keys - the spot key cannot read futures.

1. Log in to Kraken Futures and open the profile menu → **Settings** → **API Keys**.
2. Choose **Read-only** and create the key.
3. Copy both keys.

## 3. Add them to Kryptokompis
1. **Data & setup** → **Exchanges & wallets** → **Add exchange** → **Kraken**.
2. Paste the API key and Private key. The futures keys go in the two optional fields.
3. Press **Test & save**. Kryptokompis checks the key and starts syncing.

On a PC the keys are kept in Windows' own credential store, not in a file.

## Common errors
- **"The exchange rejected the key"**: the key was not copied in full, or it was deleted at Kraken.
- **"The key works but lacks a read permission"**: one of the permissions above is missing. Edit the key at Kraken and tick it.
- **Futures missing?** Add the futures key - without it only spot is fetched.
