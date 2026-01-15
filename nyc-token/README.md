## NYC Token On Chain Forensic Analysis (Solana)

Independent on chain investigation into token minting, supply control, and liquidity behavior using Solscan.

A full annotated version of this analysis with screenshots and transaction level walkthroughs is available here:  
https://www.notion.so/NYC-Token-On-Chain-Forensic-Analysis-Solana-2e9fa05ab55580c9b352d742e714b887?source=copy_link

## Overview

This case study documents an on chain forensic analysis of the NYC token on Solana, focusing on how supply distribution and liquidity control shaped what happened after launch.

Rather than relying on price charts or social media narratives, the analysis traces wallet level behavior and liquidity movements to understand how value entered the system, how it was managed, and how it was eventually extracted.

What emerges is a structurally centralized token where liquidity control, not supply ownership, determined market outcomes.

## Tools Used

- Solscan for transaction history, token accounts, mint events, and liquidity interactions
- Dexscreener to identify the token contract and primary liquidity pool prior to on chain inspection

All observations are based entirely on publicly available on chain data.

## Methodology

The investigation followed a bottom up approach focused on structure rather than price movement.

- Identified the original token mint and authority configuration
- Traced post mint supply distribution at the wallet level
- Located the primary liquidity pool and wallets interacting with it
- Tracked liquidity additions and removals over time
- Aggregated USDC inflows and outflows to assess net value extraction

The emphasis throughout was on control and mechanics, not intent attribution.

## Key Findings

- The token was minted with a fixed supply in a single transaction, with full discretion retained by the creator wallet
- Supply was distributed across multiple wallets, creating the appearance of decentralization
- The wallet holding the majority of supply never interacted with liquidity
- A separate smaller wallet controlled nearly all liquidity actions
- Liquidity was added before public trading
- Liquidity was later removed in larger amounts than it was added back
- Net USDC extraction occurred gradually rather than in a single event

## Outcome

The market remained technically tradable but economically fragile.

Liquidity depth was insufficient for reliable exits, and price stability depended almost entirely on the continued participation of a single operational wallet.

## Notes

- Wallet attribution is based on observable on chain behavior only
- No assumptions are made about identity or intent
- Conclusions are limited to data visible through Solscan
