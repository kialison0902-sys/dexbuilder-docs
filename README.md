# DexBuilder Developer Docs

This directory is a deployable bilingual Mintlify documentation project for DexBuilder's public developer documentation.

English is the default language. Simplified Chinese pages live under `zh/` with one-to-one navigation parity. Localized OpenAPI references live under `openapi/zh/`.

## Audiences

- Trading users and application developers integrating market data, orders, positions, and account data.
- Builder project teams onboarding users, managing funds and settlement, configuring fees, and reconciling revenue.

## Content status

- `openapi/trading-v1.yaml` and `openapi/zh/trading-v1.yaml` document the currently confirmed Aden-compatible perpetual REST surface.
- `openapi/builder-preview.yaml` and `openapi/zh/builder-preview.yaml` are the English and Chinese versions of a proposed public Builder contract and are clearly marked Preview.
- All production URLs, signing fields, schemas, limits, and state machines must be checked against the implementation before removing a Preview label.

## Preview locally

Install the Mintlify CLI with `npm i -g mint`, run `mint dev` from this directory, and open the local URL shown by the CLI. Mintlify currently requires Node.js 20.17 or later.

## Publish

1. Create a Mintlify project and connect the repository directory.
2. Use a test subdomain for review.
3. Configure `docs.dexbuilder.com` after content and API review.
4. Add a **Developers** link to the main DexBuilder navigation.
5. Validate both OpenAPI files and every navigation path in CI before publishing.

## GitBook option

The Markdown/MDX content can be migrated to GitBook through Git Sync. GitBook can import the OpenAPI files to generate interactive endpoint pages. Mintlify is the default here because Orderly currently uses Mintlify and this structure mirrors that documentation experience.
