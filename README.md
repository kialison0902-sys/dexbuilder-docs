# DexBuilder Developer Docs

This directory is a deployable bilingual Mintlify documentation project for DexBuilder's public developer documentation.

English is the default language. Simplified Chinese pages live under `zh/` with one-to-one navigation parity. The localized Trading OpenAPI reference lives under `openapi/zh/`.

## Audiences

- Trading users and application developers integrating market data, orders, positions, and account data.
- Builder teams planning user onboarding, funds, settlement, fees, and revenue integrations.

## Content status

- `openapi/trading-v1.yaml` and `openapi/zh/trading-v1.yaml` document the published DexBuilder perpetual REST surface based on the Aden operator API.
- `resources/builder-api-alignment.mdx` and its Chinese counterpart map the Builder capabilities documented by Orderly. A `◇` means DexBuilder still requires engineering work and has not published that operation.
- A Builder operation becomes callable documentation only after its DexBuilder route, authentication, signing, schemas, errors, environment, and end-to-end behavior are confirmed.

## Run locally

Install the Mintlify CLI with `npm i -g mint`, run `mint dev` from this directory, and open the local URL shown by the CLI. Mintlify currently requires Node.js 20.17 or later.

## Publish

1. Create a Mintlify project and connect the repository directory.
2. Use a test subdomain for review.
3. Configure `docs.dexbuilder.com` after content and API review.
4. Add a **Developers** link to the main DexBuilder navigation.
5. Validate both localized Trading OpenAPI files and every navigation path in CI before publishing.

## GitBook option

The Markdown/MDX content can be migrated to GitBook through Git Sync. Mintlify is the default because it supports the documentation and interactive Trading API experience used here.
