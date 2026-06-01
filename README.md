# VIT Autonomous Agent Swarm

**22 specialised AI agents** orchestrating intelligence, verification, and market operations for the VIT Network.

[![Python](https://img.shields.io/badge/Python-3.11-blue?style=flat-square&logo=python)](https://python.org)
[![Agents](https://img.shields.io/badge/Agents-22_Active-blueviolet?style=flat-square)]()

## Agent Registry

| Agent | Cycle | Role |
|-------|-------|------|
| `live-match-tracker` | 30s | Tracks live fixture updates and triggers settlements |
| `weight-optimizer` | 6h | Rebalances ensemble model weights from outcomes |
| `oracle-sentinel` | 5m | Monitors on-chain oracle health and verifies results |
| `kyc-screener` | 10m | Processes KYC queue and escalates high-risk users |
| `fraud-reviewer` | 15m | Anomaly detection across wallet and betting activity |
| `market-scout` | 1h | Discovers new markets and evaluates signal quality |
| `clv-tracker` | 1h | Calculates closing line value for all predictions |
| `academic-tutor` | 6h | Generates personalised learning content |
| `audit-sentinel` | 30m | Monitors smart contract events and on-chain state |
| `pricing-engine` | 5m | Updates VITCoin price from supply/demand/revenue |
| `... 12 more` | | |

## Architecture

All agents extend `BaseAgent` with a `_run_cycle()` method. The swarm orchestrator manages lifecycle, error recovery, and lazy loading for memory efficiency.
