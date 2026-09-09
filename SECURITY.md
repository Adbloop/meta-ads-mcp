# Security Policy

## Reporting a vulnerability

If you find a security issue in the Adbloop Meta Ads MCP or the Adbloop
service, please report it privately — do **not** open a public issue.

Email: **support@nishithpandya.com**

Please include steps to reproduce and the potential impact. We aim to
acknowledge reports within 72 hours.

## Scope

- This repository contains documentation, configuration, and the connector
  manifest only. It contains no credentials and no proprietary server code.
- The Adbloop service runs hosted. Authentication is via OAuth; the MCP reuses
  the Meta connection you authorize inside Adbloop. Adbloop never asks you to
  paste API keys or tokens into this repo or into your AI assistant.

## For users

- Never paste Meta access tokens, app secrets, or API keys into a chat, a
  config file, or an issue in this repo. Adbloop does not require them.
- Campaigns can be created **paused** by default — review before anything
  spends. See [docs/safety.md](./docs/safety.md).
