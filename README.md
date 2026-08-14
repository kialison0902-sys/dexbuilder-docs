# DexBuilder Developer Docs

This directory contains the bilingual Mintlify site for DexBuilder's public developer documentation.

English is the default language. Simplified Chinese pages live under `zh/`. Localized Trading OpenAPI specifications live under `openapi/zh/`.

## Information architecture

- Home and Introduction explain the platform and core trading model.
- Build on DexBuilder covers onboarding, authentication, trading, asset settlement, and Builder operations as one integration journey.
- API Reference contains the interactive Trading OpenAPI specification.
- Developer tools, Troubleshooting, and Release notes support implementation and production operations.

## Run locally

Install the Mintlify CLI with `npm i -g mint`, run `mint dev` from this directory, and open the local URL shown by the CLI.

## Publish

1. Validate `docs.json`, internal links, and both Trading OpenAPI files.
2. Commit changes to the connected GitHub repository.
3. Confirm the Mintlify deployment in English and Chinese.
