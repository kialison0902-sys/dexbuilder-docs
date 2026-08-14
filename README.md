# DexBuilder Developer Docs

This directory contains the bilingual Mintlify site for DexBuilder's public developer documentation.

English is the default language. Simplified Chinese pages live under `zh/`. Localized Trading OpenAPI specifications live under `openapi/zh/`.

## Documentation areas

- Trading API for market data, accounts, positions, orders, and history.
- Core integration flows for accounts, wallet authorization, deposits, withdrawals, PnL settlement, and internal transfers.
- Builder API guides for user data, fee settings, revenue settlement, order tags, campaigns, and referrals.

## Run locally

Install the Mintlify CLI with `npm i -g mint`, run `mint dev` from this directory, and open the local URL shown by the CLI.

## Publish

1. Validate `docs.json`, internal links, and both Trading OpenAPI files.
2. Commit changes to the connected GitHub repository.
3. Confirm the Mintlify deployment in English and Chinese.
