# Economic Simulation Lab

Updated: 2026-11-22.

A standalone desktop simulation of token supply, AMM market making, synthetic COIN/USD liquidity pools, staking, validator nodes, reward distribution, agent/user trading, simulated site revenue, contests and price history.

The simulation is local and uses toy balances, not real blockchain transactions or real currency. It is not connected to Commonworld Testnet or any live market.

## Run

Python 3.10+:

```bash
python -m pip install -r requirements.txt
python code.py
```

The desktop window is 1300x800, showing node statistics, synthetic token balances, exchange reserves and price history. The Management menu supports user/node management, buy/sell actions, contests and system trades. Font rendering uses an installed system sans-serif font.

## Included models

Token supply 5,000,000,000 COIN; synthetic USD reserves and 0.3% AMM trade fees; staking and rewards; market-maker reaction with panic-buy and fair-value policy; local synthetic trading and market information.

Economic parameters are illustrative, not empirically calibrated. This version recreates a compact standalone economic simulation for demonstration and experiments; future HELIOS development remains a separate planned system.

## Checks

`python -m py_compile code.py` checks syntax. An interactive Pygame desktop smoke test is still required; source packaging alone does not confirm runtime behavior.
