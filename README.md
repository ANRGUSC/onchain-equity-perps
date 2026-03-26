# Beyond Brokerage Hours: Credibly Neutral 24/7 Equity Markets on Ethereum

**Platform Commitment, Perpetual Instrument Design, and Decentralized Value Allocation for Tokenized Equity Access**

Hardhik Mohanty | [University of Southern California, Viterbi School of Engineering](https://viterbischool.usc.edu/) | [hmohanty@usc.edu](mailto:hmohanty@usc.edu)

Advisor: [Prof. Bhaskar Krishnamachari](https://ceng.usc.edu/~bkrishna/)

*Ethereum Foundation PhD Fellowship -- RFP: Economic Models Enabled by Decentralized Trust Systems*

---

## Abstract

Centralized equity markets operate on fixed schedules under the discretionary control of platform operators who can unilaterally alter fees, access rules, and value-sharing arrangements. This creates well-documented commitment failures: traders, liquidity providers, and third-party integrators who make relationship-specific investments face hold-up risk because the platform retains residual control. Ethereum provides the composability, public verifiability, smart-contract durability, and credibly neutral interface layer needed for these participants to make such investments without fear of ex-post platform discretion.

This project develops a formal economic and computational framework for **equity-linked perpetuals on Ethereum**, using tokenized spot equity as a comparison benchmark. The research combines incomplete-contract theory, platform economics, and dynamic mean-field market microstructure to identify the conditions under which decentralized commitment improves participation, liquidity, and welfare, and to design value-allocation mechanisms that minimize rent extraction across all participant classes.

## Research Motivation

Institutional appetite for tokenized financial assets on Ethereum is strong and growing: BlackRock's BUIDL fund reached ~$2.9B AUM within its first year, Robinhood launched tokenized stocks on an Ethereum L2, the DTCC received an SEC no-action letter for a securities tokenization pilot, and Cboe has filed to launch near-24x5 U.S. equities trading. These developments make the core research questions commercially urgent rather than speculative.

No single centralized operator can replicate Ethereum's combination of composability across independent front ends, public verifiability of rule enforcement, smart-contract durability, and credible neutrality -- without reintroducing discretionary trust assumptions. This project asks: **when do these properties make equity-linked perpetuals economically superior to centralized alternatives for 24/7 global equity access?**

## Core Research Questions and Hypotheses

1. **When does decentralized trust increase participation and liquidity enough to outweigh additional on-chain frictions?**
2. **When do equity-linked perpetuals dominate spot tokenization as the most scalable form of 24/7 equity exposure?**
3. **How should trading revenues and control rights be allocated so that the market remains open, composable, and resistant to rent extraction?**

**Hypotheses:**
- **H1.** Credibly neutral fee and access commitments increase third-party liquidity provision and reduce rent extraction relative to centralized extended-hours platforms.
- **H2.** Equity-linked perpetuals are a more scalable form of 24/7 global equity exposure than spot-token wrappers in settings where corporate-action and register-management frictions are material.
- **H3.** A hybrid design combining continuous trading with event-sensitive auction windows produces better price-discovery efficiency and lower adverse-selection costs than pure continuous trading during low-liquidity hours.

## Methodology Overview

The project proceeds in four linked workstreams:

| Workstream | Focus | Approach |
|---|---|---|
| **WS1: Organizational Model** | Centralized vs. decentralized equity market organization | Incomplete-contracts framework (Grossman-Hart-Moore), platform economics |
| **WS2: Instrument Design** | Spot tokens vs. equity-linked perpetuals | Contract-theoretic comparison of ownership, entitlement, and synthetic exposure |
| **WS3: Dynamic Microstructure** | 24/7 market equilibrium with heterogeneous agents | Multi-population mean-field game model (extending prior MFG work on stablecoins) |
| **WS4: Empirical Calibration** | Model validation against real market data | After-hours equity data (NYSE TAQ/WRDS), crypto perpetual data (Binance, dYdX), tokenized equity on-chain data |

The model includes six agent classes: global directional traders, passive/active liquidity providers, market makers, front-end operators, oracle/attestation providers, and protocol maintainers.

## Planned Datasets

- **After-hours U.S. equity data** -- NYSE TAQ database via WRDS (bid-ask spreads, depth, trade counts, price impact around earnings/FOMC releases)
- **24/7 crypto perpetual market data** -- Funding rates, basis time series, order-book snapshots, and liquidation events from Binance and dYdX (public APIs)
- **Tokenized equity platform data** -- On-chain transaction data for Robinhood tokenized stocks (Arbitrum) and Kraken xStocks (Backed Finance), via Dune Analytics and Etherscan

## Deliverables

- A **theoretical platform model** of centralized vs. decentralized equity market organization under incomplete contracting and user lock-in
- A **dynamic market-microstructure model** of traders, LPs, market makers, and arbitrageurs in 24/7 equity-linked perpetual markets, using mean-field game methodology
- A **mechanism-design blueprint** for credibly neutral value allocation and liquidity incentives
- At least **one major paper submission** to a leading venue in financial economics, blockchain, or market design
- **Open-source simulation and calibration code** (this repository)
- A **practitioner-facing design memo** for Ethereum builders and policymakers

## Timeline

| Phase | Months | Focus |
|---|---|---|
| **Milestone 1** | 1--3 | Literature synthesis, institutional mapping, data pipeline construction |
| **Milestone 2** | 3--6 | Formal organizational model (incomplete contracts + platform design) |
| **Milestone 3** | 6--10 | Dynamic MFG market-microstructure model, calibration, counterfactual experiments |
| **Milestone 4** | 10--12 | Paper submission, open-source release, design memo, dissemination |

## Related Publications

1. **H. Mohanty** and B. Krishnamachari, "Who Restores the Peg? A Mean-Field Game Approach to Model Stablecoin Market Dynamics," *arXiv:2601.18991*, 2026. Accepted at *IEEE ICBC 2026*. [[arXiv]](https://arxiv.org/abs/2601.18991)

2. **H. Mohanty**, G. Zaarour, and B. Krishnamachari, "Proactive Market Making and Liquidity Analysis for Everlasting Options in DeFi Ecosystems," *IEEE ICBC 2025*. DOI: [10.1109/ICBC64466.2025.11114454](https://doi.org/10.1109/ICBC64466.2025.11114454)

3. Z. Feng, **H. Mohanty**, and B. Krishnamachari, "Modeling and Analysis of Crypto-Backed Over-Collateralized Stable Derivatives in DeFi," *Frontiers in Blockchain*, vol. 7, 2024. DOI: [10.3389/fbloc.2024.1392812](https://doi.org/10.3389/fbloc.2024.1392812)

## Author

**Hardhik Mohanty**
PhD Student, Electrical and Computer Engineering
University of Southern California (USC)
Advisor: Prof. Bhaskar Krishnamachari

- [Personal Website](https://hardhik-99.github.io/hmohanty/)
- [Google Scholar](https://scholar.google.com/citations?user=99B3RkcAAAAJ&hl=en)
- [ANRG Lab](https://github.com/ANRGUSC)

## License

This project is licensed under the [MIT License](LICENSE).

All research outputs will be open-access and permissively licensed, consistent with Ethereum Foundation fellowship requirements.
