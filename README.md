# DexBuilder Developer Docs

This directory contains the bilingual Mintlify site for DexBuilder's public developer documentation.

English is the default language. Simplified Chinese pages live under `zh/`. Localized Trading OpenAPI specifications live under `openapi/zh/`.

## Information architecture

- Introduction combines the product landing page, product suite, core capabilities, platform architecture, accounts, and core trading concepts.
- Build on DexBuilder covers onboarding, authentication, trading, asset settlement, and Builder operations as one integration journey.
- API Reference contains the interactive Trading OpenAPI specification.
- Developer tools covers environments, API conventions, and integration tooling.
- Troubleshooting supports implementation and production operations.
- Release notes records product capabilities for perpetual DEX, prediction market, and event contract products.

## Run locally

Install the Mintlify CLI with `npm i -g mint`, run `mint dev` from this directory, and open the local URL shown by the CLI.

## Publish

1. Validate `docs.json`, internal links, and both Trading OpenAPI files.
2. Commit changes to the connected GitHub repository.
3. Confirm the Mintlify deployment in English and Chinese.
