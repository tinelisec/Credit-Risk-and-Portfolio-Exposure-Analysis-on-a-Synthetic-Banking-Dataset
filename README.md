# Risk-Oriented Analysis of a Synthetic Commercial Banking Dataset

A self-directed portfolio project applying practical credit risk analysis skills to a synthetic commercial banking dataset, built for finance internship applications, particularly risk management roles.

## Overview

The dataset contains 1.26 million records spanning customers, accounts, loans, cards, transactions, and merchants. Before any analysis, the dataset is checked for data quality and generation artifacts, it shows clear signs of synthetic generation (uniform distributions, flat interest rate pricing across credit score bands, identical concentration metrics across account types) and carries real limitations, including missing fields like loan status and default history. These are flagged upfront rather than left to surface partway through the analysis.

## What this project covers

- **Data quality assessment**: null checks, duplicate detection, and synthetic-pattern identification before trusting any downstream numbers
- **Customer and account base profiling**: credit score distribution, geography, account type mix
- **Portfolio concentration**: exposure by account type, top-account and top-merchant concentration, HHI
- **Credit risk analysis**: whether interest rate pricing actually reflects credit risk, high-risk exposure sizing, loan-to-balance ratio outliers
- **Transaction behavior**: monthly trends, dormant account detection, same-day activity spikes

## Approach

All data collection, calculations, and visualizations were built using SQL and Python. The goal is to demonstrate the full analytical process end to end: checking data quality before trusting it, applying risk vocabulary and methodology correctly, and being explicit about where the analysis's conclusions can and can't be trusted, given the dataset's synthetic origin.

A SQL query appendix is included in the full report, showcasing window functions, multi-step CTEs, and weighted aggregations used throughout the analysis.
