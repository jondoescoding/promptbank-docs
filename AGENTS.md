# Prompt Bank documentation guide

## Purpose

This repository owns the public Prompt Bank documentation at
`https://docs.promptbank.club`.

Prompt Bank helps people discover, save, organize, share, and reuse AI prompts.
It also connects those prompts to AI generation.

## Sources of truth

- Customer documentation lives in the MDX files in this repository.
- Site navigation, theme, logos, and global settings live in `docs.json`.
- The current public API contract is `https://www.promptbank.club/api/v1/openapi.json`.
- Product behavior comes from the Prompt Bank application repository at
  `C:/Users/Jonathan/Documents/CODING/PERSONAL/thepromptbank`.
- A route, type, test fixture, or marketing statement does not prove that a
  workflow works. Verify the complete workflow before you document it as ready.

## Writing rules

- Use ASD-STE100 Simplified Technical English.
- Use active voice and address the reader as `you`.
- Keep one idea in each sentence.
- Use sentence case for headings.
- Format interface labels in bold and code, paths, fields, and commands as code.
- Define a technical term in plain language when you first use it.
- Use concrete examples that match the production API.
- Keep internal routes, service credentials, bot accounts, infrastructure, and
  administrator procedures out of public documentation.

## Product terms

- Use `Prompt Bank` for the product.
- Use `prompt` for reusable AI instructions.
- Use `vault` for a collection that organizes prompts.
- Use `generation` for media created from a prompt.
- Do not describe unavailable audio, video, billing, publishing, or marketplace
  workflows as available.

## Design

- Keep the Mintlify `luma` theme unless the user requests another theme.
- Use `#ffff00` as the primary and dark-mode brand colour.
- Use `#767600` as the accessible light-mode brand colour.
- Keep `https://www.promptbank.club` as the main product action.

## Update workflow

1. Run `git status --short` and preserve unrelated changes.
2. Pull the current `main` branch before editing when the tree is clean.
3. Compare API documentation with the current OpenAPI contract and application
   behavior.
4. Validate `docs.json`, links, MDX syntax, and the Mintlify build with a
   supported Node.js LTS release.
5. Inspect desktop and mobile screenshots. Review browser console and page
   errors.

Mintlify deploys commits pushed to `jondoescoding/promptbank-docs`, branch
`main`. A local edit is not a production release. Do not commit, push, or change
Mintlify settings without authorization. After an authorized push, confirm a
successful Mintlify activity entry and verify `https://docs.promptbank.club`.
