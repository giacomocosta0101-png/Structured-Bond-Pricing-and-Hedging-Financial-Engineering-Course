# Structured Bond Pricing & Hedging (LMM / BMM)

**Assignment 5** · MATLAB · Financial Engineering course, Politecnico di Milano

Pricing and risk management of a **EUR 50M 10-year structured bond** with capped and digital coupons, and pricing of an exotic cap under the **Bond Market Model**.

## What we did

- **Caplet spot-volatility stripping**: 79 × 13 surface from market flat cap volatilities (1–20y, 13 strikes).
- **Structured bond** with embedded caplets and digitals — fair upfront 13.18%.
- **Risk**: bucket DV01 on 60 curve instruments, coarse-grained DV01 and total vega (−EUR 142.5k per +1% vol).
- **Hedging**: delta hedge with 2y/6y/10y par swaps, vega hedge with 6y/10y ATM caps.
- **Digital risk**: call-spread smile correction moves the upfront by 23 bp.
- **Exotic cap on Libor differences** under BMM: caplet-by-caplet calibration and spot-measure Monte Carlo on 16 correlated forward bonds.

## Repository structure

| Path | Content |
|---|---|
| `runAssignment5_Group5.m` | Main script |
| `bootstrap/` | Discount-curve bootstrap (depos, futures, swaps) |
| `ex_1/Point a … g/` | Vol stripping, pricing, DV01, vega, delta/vega hedging, digital risk |
| `ex_2/` | Exotic cap under the Bond Market Model |
| `REPORT_Assignment5_FE_Group5.pdf` | Report |

## How to run

Open the folder in MATLAB (R2023b or later) and run `runAssignment5_Group5.m`. It adds the sub-folders to the path and executes every exercise in order.

## Team

Gabriele Alippi, Elisa Colombo, Simone Colombo, Giacomo Costa

Part of the **Financial Engineering** course (Prof. R. Baviera) — M.Sc. in Mathematical Engineering, Quantitative Finance, Politecnico di Milano, A.Y. 2025/26.
