# LedgerFlow
![LedgerFlow logo](assets/logo.png)

Tokenized invoice financing for B2B cross-border trade on Solana.

## Overview

LedgerFlow lets enterprises mint their unpaid invoices as on-chain tokens and get instant stablecoin financing from a liquidity pool, bypassing slow bank factoring. Companies get working capital in minutes while investors earn yield backed by real receivables.

## Problem

Traditional invoice factoring is slow, opaque, and expensive, especially for cross-border B2B trade. SMEs and mid-size enterprises often wait weeks for banks to advance funds against invoices they've already earned, tying up working capital they need to grow.

## Solution

LedgerFlow tokenizes verified invoices as RWA tokens and lets a permissionless lending pool instantly advance stablecoins against them, with automated repayment when the invoice is settled. This gives enterprises fast access to capital and gives stablecoin holders a yield source backed by real-world receivables.

## Features (MVP)

- Invoice upload & on-chain verification via oracle/KYB partner
- Mint invoice as RWA token representing the receivable
- Instant stablecoin advance from liquidity pool at a risk-based rate
- Automated repayment & yield distribution when invoice is paid
- Dashboard for enterprises and liquidity providers

## Tech Stack

- Anchor (Solana smart contracts)
- Solana Program Library
- USDC
- Chainlink / Pyth oracles
- Next.js (frontend)
- Supabase (off-chain data)

## How It Works

```
Enterprise -> Upload Invoice -> KYB/Oracle Verification
                                   |
                                   v
                        Mint Invoice RWA Token (Solana)
                                   |
                                   v
                 Liquidity Pool (USDC) --- advances stablecoins --> Enterprise
                                   |
                        Invoice Paid by Buyer
                                   |
                                   v
          Smart Contract Auto-Repayment --- yield --> Liquidity Providers
```

All minting, lending, and repayment logic runs through Anchor programs on Solana. The Next.js dashboard, backed by Supabase, lets enterprises track invoice status and lets liquidity providers monitor deployed capital and earned yield.

## Roadmap

- Partner with a KYB/credit-scoring provider for invoice verification
- Pilot with 5-10 SMEs in a specific trade corridor
- Add a secondary market for trading invoice tokens

## Pitch

- [Pitch deck (PDF)](docs/pitch.pdf)
- [Pitch script](docs/pitch-script.md)

## Team

- Name — Role (GitHub: @handle)
- Name — Role (GitHub: @handle)
- Name — Role (GitHub: @handle)

Built for the Colosseum hackathon.

---

🎬 Pitch video: [docs/pitch-video.webm](docs/pitch-video.webm)
