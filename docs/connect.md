# Connect Adbloop Meta Ads MCP

Before you start: create a free account at **[app.adbloop.com](https://app.adbloop.com)** and connect your Meta (Facebook) ad account. The MCP reuses that connection — there are no API keys to copy anywhere.

---

## Claude

Adbloop connects to Claude over one-click OAuth (Claude Desktop and Claude on the web, on plans that support connectors).

1. Open **Settings → Connectors** in Claude.
2. Add the **Adbloop** connector (or paste the Adbloop MCP URL if prompted).
3. Approve the OAuth sign-in — you'll be sent to Adbloop and back.
4. Start a chat and ask Claude to list your ad accounts to confirm it's live.

No JSON editing required. (For older Claude Desktop builds that use a config file, add Adbloop as a remote MCP server per Anthropic's current connector docs — Adbloop is a hosted, streamable-HTTP remote, so you do not run anything locally.)

---

## ChatGPT

Adbloop works with ChatGPT via **Developer Mode / connectors** (availability depends on your ChatGPT plan).

1. Enable **Developer Mode** (Settings → Connectors / Advanced).
2. Add a new connector pointing at the Adbloop MCP.
3. Complete the OAuth sign-in to Adbloop.
4. Ask ChatGPT to list your ad accounts to confirm.

---

## Cursor & other MCP clients

Any MCP client that supports **remote (streamable-HTTP) servers with OAuth** can connect. Add Adbloop as a remote MCP server using the endpoint from [adbloop.com/mcp](https://adbloop.com/mcp/), then authorize via OAuth.

---

## Verify it works

Ask your assistant:

> "List my connected ad accounts."

If it returns your Meta ad accounts, you're connected. Next, try a safe dry run:

> "Validate a $10/day Facebook conversions campaign for account &lt;name&gt; — don't create it, just check it."

See more in [examples/prompts.md](../examples/prompts.md).

---

## Troubleshooting

- **No accounts returned?** Sign in at [app.adbloop.com](https://app.adbloop.com) and confirm your Meta ad account is connected there first.
- **Connector won't authorize?** Make sure you're logged into the same Adbloop account in your browser, then retry the OAuth step.
- Still stuck? See [SECURITY.md](../SECURITY.md) for contact, or email support@nishithpandya.com.
