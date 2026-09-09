# Safety: letting AI manage a live Meta Ads account

Giving an AI assistant write access to a live Facebook/Instagram ad account is a real risk — budget mistakes, invalid targeting, duplicate or malformed campaigns, rate-limit throttling, and hallucinated IDs are all failure modes people hit in practice. Here's how Adbloop is built to prevent them.

## Guardrails Adbloop applies

- **Paused by default.** Campaigns can be created paused so nothing spends until you review and turn them on.
- **Pre-flight validation.** `validate_campaigns` checks against Meta's rules *before* anything is created — objective/goal/destination compatibility, targeting, budgets, creative requirements.
- **Spend guardrails.** `get_guardrails` reflects per-campaign and account-level spend caps, so a bulk run can't blow past a ceiling.
- **Capacity & estimate checks.** `check_capacity` and `estimate_bulk_create` show rate-limit headroom and batch size before you commit, avoiding Meta API throttling and partial-batch failures.
- **108 documented Meta API fixes.** Adbloop is hardened against the concrete ways Meta bulk operations fail — the reliability layer runs server-side.

## Recommended workflow

1. Ask your assistant to **validate** (or dry-run) first.
2. Create **paused**.
3. Review in the [Adbloop dashboard](https://app.adbloop.com) or Meta Ads Manager.
4. Resume / turn live when you're happy.

## What Adbloop never does

- It never asks you to paste Meta tokens, app secrets, or API keys into your AI assistant or into this repo. Authentication is OAuth, reusing the Meta connection you authorized inside Adbloop.
