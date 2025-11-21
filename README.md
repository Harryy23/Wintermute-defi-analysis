Wintermute DeFi Trading Analysis
Analysis of Wintermute's decentralized trading activity using on-chain blockchain data. Built for the Syntagma Labs Quant Researcher technical assessment.

What This Project Does
This repository contains a Python-based analysis of 437,000 blockchain transactions from Wintermute's DeFi operations on April 8, 2025. The goal was to understand how a major market maker operates across decentralized exchanges, which blockchains they prioritize, and what their trading patterns reveal about institutional DeFi strategies.

Main Findings
Trading Focus:

87% of Wintermute's activity happens on DeFi protocols (vs centralized exchanges)

41% of volume is in stablecoins (USDC and USDT), suggesting they're mainly providing liquidity rather than speculating

They're active on 18 different DeFi protocols, with Uniswap handling 41% of total volume

Multi-Chain Strategy:

Ethereum: 50% of volume, but only 18K transactions (avg $23,700 per trade → institutional-grade activity)

Solana: 22% of volume with 261K transactions (avg $726 per trade → high-frequency market-making)

Base, Arbitrum, and other L2s make up the remaining 28%

Timing:

Peak trading happens 2:00-4:00 UTC (9-11 PM EST), indicating US market hours drive most activity

Secondary peak at 11:00 UTC suggests European traders are also active

Methodology
Entity Classification:
I classified 84 unique counterparties into categories (DeFi, CEX, MEV builders, etc.) using:

Pre-labeled entity names from the dataset

Blockchain explorers (Etherscan, Solscan) for verification

Public DeFi protocol documentation

12.5% of entities couldn't be classified due to missing labels.

Analysis Approach:

Aggregated token volumes and transaction frequencies

Compared activity across blockchains (Ethereum, Solana, Base, etc.)

Identified temporal patterns (hourly trading volume)

Built scatter plots to visualize relationships between frequency and volume

Limitations
This analysis has a few constraints worth noting:

Single-day snapshot: 11.5 hours of data may not reflect longer-term strategies

Incomplete classification: 12.5% of transactions involve unlabeled entities

No profitability analysis: The dataset doesn't include enough info to calculate P&L

No slippage data: Can't assess execution quality or price impact

Future work could extend this to multi-day analysis, classify unknown entities using contract verification, and add profitability metrics.

Key Takeaways for Quant Research
If you're looking at this as a hiring manager or researcher, here's what matters:

Dual-market approach: Wintermute runs institutional trades on Ethereum and high-frequency retail strategies on Solana—distinct models optimized for each chain's characteristics.

Liquidity-first strategy: Stablecoin dominance (41% of volume) confirms their primary role is market-making, not directional trading.

Infrastructure maturity: Active presence on 6+ blockchains with 18 DeFi protocols shows sophisticated cross-chain operations.

Timing matters: US evening hours (2-4 UTC) drive peak activity, likely because retail and institutional traders overlap during high-liquidity windows.

Last updated: November 21, 2025
