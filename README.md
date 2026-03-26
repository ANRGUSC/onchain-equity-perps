<div align="center">

# Beyond Brokerage Hours

### Credibly Neutral 24/7 Equity Markets on Ethereum

*Platform Commitment, Perpetual Instrument Design, and Decentralized Value Allocation for Tokenized Equity Access*

</div>

<br>

<p align="center"><em>Application to Ethereum Foundation PhD Fellowship -- RFP: Economic Models Enabled by Decentralized Trust Systems</em></p>

---

## Overview

Centralized equity markets operate on fixed schedules under the discretionary control of platform operators who can unilaterally alter fees, access rules, and value-sharing arrangements. This creates well-documented commitment failures: traders, liquidity providers, and third-party integrators who make relationship-specific investments face **hold-up risk** because the platform retains residual control.

**Ethereum** provides the composability, public verifiability, smart-contract durability, and credibly neutral interface layer needed for these participants to make such investments without fear of ex-post platform discretion. No single centralized operator can replicate these properties without reintroducing discretionary trust assumptions.

This project develops a formal economic and computational framework for **equity-linked perpetuals on Ethereum**, combining incomplete-contract theory, platform economics, and dynamic mean-field market microstructure to identify the conditions under which decentralized commitment improves participation, liquidity, and welfare.

---

## Motivation

| Development | Signal |
|:---|:---|
| BlackRock BUIDL fund | ~$2.9B AUM within first year on Ethereum |
| Robinhood tokenized stocks | Launched on Ethereum L2 (Arbitrum) for EU users |
| DTCC no-action letter | SEC-approved pilot for securities tokenization |
| Cboe 24x5 filing | Near round-the-clock U.S. equities trading |
| SEC staff statement (Jan 2026) | Taxonomy for tokenized vs. issuer-tokenized securities |

---

## Research Questions & Hypotheses

<table>
<tr><th width="60">ID</th><th>Question</th></tr>
<tr><td><b>Q1</b></td><td>When does decentralized trust increase participation and liquidity enough to outweigh additional on-chain frictions?</td></tr>
<tr><td><b>Q2</b></td><td>When do equity-linked perpetuals dominate spot tokenization as the most scalable form of 24/7 equity exposure?</td></tr>
<tr><td><b>Q3</b></td><td>How should trading revenues and control rights be allocated so that the market remains open, composable, and resistant to rent extraction?</td></tr>
</table>

<br>

**Hypotheses:**

- **H1.** Credibly neutral fee and access commitments increase third-party liquidity provision and reduce rent extraction relative to centralized extended-hours platforms.
- **H2.** Equity-linked perpetuals are a more scalable form of 24/7 global equity exposure than spot-token wrappers in settings where corporate-action and register-management frictions are material.
- **H3.** A hybrid design combining continuous trading with event-sensitive auction windows produces better price-discovery efficiency and lower adverse-selection costs than pure continuous trading during low-liquidity hours.

---

## Methodology

The project proceeds in **four linked workstreams** that build progressively from institutional theory to computational modeling to empirical validation.

```
WS1  Organizational Model        Incomplete contracts (Grossman-Hart-Moore) + platform economics
 |
WS2  Instrument Design           Spot tokens vs. equity-linked perpetuals (contract theory)
 |
WS3  Dynamic Microstructure      Multi-population mean-field game model
 |
WS4  Empirical Calibration       After-hours equity, crypto perps, on-chain tokenized equity
```

The model includes **six agent classes**: global directional traders, passive/active liquidity providers, market makers, front-end operators, oracle/attestation providers, and protocol maintainers.

**Planned datasets:**

| Source | Data | Access |
|:---|:---|:---|
| NYSE TAQ (WRDS) | After-hours bid-ask spreads, depth, trade counts, price impact | USC institutional subscription |
| Binance & dYdX | Funding rates, basis, order-book snapshots, liquidation events | Public REST & WebSocket APIs |
| Arbitrum / Etherscan | Robinhood tokenized stock transactions, Kraken xStocks (Backed Finance) | Dune Analytics, on-chain |

---

## Deliverables

| Output | Description |
|:---|:---|
| Theoretical model | Centralized vs. decentralized equity market organization under incomplete contracting |
| MFG microstructure model | Dynamic mean-field game of traders, LPs, MMs, and arbitrageurs in 24/7 equity markets |
| Mechanism-design blueprint | Credibly neutral value allocation and liquidity incentives |
| Academic paper | Submission to a leading venue in financial economics, blockchain, or market design |
| Open-source code | Simulation and calibration codebase (this repository) |
| Design memo | Practitioner-facing document for Ethereum builders and policymakers |

---

## Timeline

```
Month   1          3          6          10         12
  |----------|----------|----------|----------|
  MS1        MS2        MS3                   MS4
  Literature  Formal     MFG Model +          Paper +
  + Data      Org Model  Calibration          Release
```

| Milestone | Months | Focus |
|:---|:---:|:---|
| **MS1** -- Literature & Data | 1--3 | Structured literature review, institutional case studies, data pipeline construction |
| **MS2** -- Formal Model | 3--6 | Incomplete-contracts + platform-design model, threshold conditions, welfare results |
| **MS3** -- Computational Model | 6--10 | Multi-population MFG implementation, calibration, counterfactual experiments |
| **MS4** -- Dissemination | 10--12 | Paper submission, open-source release, design memo, community presentation |

---

## Related Publications

1. **H. Mohanty** and B. Krishnamachari, "Who Restores the Peg? A Mean-Field Game Approach to Model Stablecoin Market Dynamics," *arXiv:2601.18991*, 2026. Accepted at *IEEE ICBC 2026*.
   [[arXiv]](https://arxiv.org/abs/2601.18991)

2. **H. Mohanty**, G. Zaarour, and B. Krishnamachari, "Proactive Market Making and Liquidity Analysis for Everlasting Options in DeFi Ecosystems," *IEEE ICBC 2025*.
   [[DOI]](https://doi.org/10.1109/ICBC64466.2025.11114454)

3. Z. Feng, **H. Mohanty**, and B. Krishnamachari, "Modeling and Analysis of Crypto-Backed Over-Collateralized Stable Derivatives in DeFi," *Frontiers in Blockchain*, vol. 7, 2024.
   [[DOI]](https://doi.org/10.3389/fbloc.2024.1392812)

---

## License

This project is licensed under the [MIT License](LICENSE).

---

<div align="center">
<sub>Built at the <a href="https://anrg.usc.edu/">Autonomous Networks Research Group</a>, USC</sub>
</div>
