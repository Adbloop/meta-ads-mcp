# Tools reference

The Adbloop Meta Ads MCP exposes 22 tools for Facebook & Instagram (Meta) Ads. Descriptions below say **what** each tool does — the validation, error-recovery, and rate-limit handling that make bulk operations reliable run server-side.

## Create & launch

| Tool | What it does |
|---|---|
| `create_campaign` | Create one Facebook/Instagram campaign end to end. |
| `create_structured` | Create a fully specified campaign → ad set → ad in one structured call. |
| `bulk_create_campaigns` | Create many campaigns in a single account in one request. |
| `bulk_create_multi_account` | Create campaigns across several ad accounts at once (agencies). |
| `add_ad_to_adset` | Add an ad to an existing ad set. |
| `list_drive_folder` | List creatives in your connected Google Drive folder to build ads from. |

## Stay safe before you spend

| Tool | What it does |
|---|---|
| `validate_campaigns` | Check campaigns against Meta's rules **before** anything goes live. |
| `estimate_bulk_create` | Preview how large a bulk batch is before running it. |
| `check_capacity` | Check rate-limit headroom / how much you can create right now. |
| `get_guardrails` | Read the spend guardrails (per-campaign and account caps) in force. |

## Manage what's running

| Tool | What it does |
|---|---|
| `pause_campaigns` | Pause one or more campaigns. |
| `resume_campaigns` | Resume paused campaigns. |
| `delete_campaigns` | Delete campaigns. |
| `update_campaign_budget` | Change a campaign's budget. |

## Read & report

| Tool | What it does |
|---|---|
| `get_ad_accounts` | List your connected Meta ad accounts. |
| `list_campaigns` | List campaigns in an account. |
| `list_adsets` | List ad sets. |
| `list_ads` | List ads. |
| `get_campaign_structure` | Get the full campaign → ad set → ad structure. |
| `get_insights` | Pull performance metrics. |
| `get_creative_library` | Browse available creatives. |
| `get_lead_forms` | List lead forms for lead-gen campaigns. |
| `search_targeting` | Look up Meta targeting options (interests, locations, etc.). |

> Full, current capabilities are listed at [adbloop.com/mcp](https://adbloop.com/mcp/).
