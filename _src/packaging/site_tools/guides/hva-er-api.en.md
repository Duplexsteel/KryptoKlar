---
title: What is an API - and is it safe to use with your crypto exchange?
date: 2026-10-17
summary: A short video (in Norwegian) on what an API is, what an API key can do, how to use it safely, and the alternatives.
order: 2
kind: guide
video: M1TyoDfgWnI
---
Many crypto apps ask for an API key. The video (in Norwegian) explains what that is, in plain words.

## In short
- **An API is the waiter between two programs.** Kryptokompis asks the exchange for your trades, and the exchange answers with the data.
- **An API key has two parts:** a public part, like a username, and a secret part, like a password. You decide what the key may do, and you can delete it whenever you like.
- **An exchange API can read, trade and withdraw.** Kryptokompis only needs to read.
- **Give the key read access only.** Then it can never trade or withdraw, even if someone got hold of it. Kryptokompis refuses Binance, Coinbase and KuCoin keys that can do more than read.
- **Rather not use an API?** Download a statement file from the exchange and import it, or fill in the template yourself.

## How to create the key at your exchange
See [the guides for each exchange](guides.html).
