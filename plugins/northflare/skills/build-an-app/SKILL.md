---
name: build-an-app
description: Build a custom Shopify app with Northflare. Use when the person wants a custom app for their Shopify store, or asks about their Northflare apps.
---

# Building a Shopify app with Northflare

Northflare builds and hosts custom Shopify apps for store owners, most of
whom are not developers. Its tools come from the Northflare connector that
this plugin adds.

1. **Sign in.** If Northflare's tools (`status`, `draft_plan`) are not
   available, the connector is waiting for the person to sign in. Never
   ask them to type a command in a terminal. In Codex, start it yourself
   by running `codex mcp login northflare`. Claude Code cannot start it
   for you: ask them to type `/mcp` in the message box, choose
   `northflare` and sign in. Either way Northflare's sign-in page opens
   in their browser, and they press **Sign in** there. If the tools still
   don't appear, ask them to start a new conversation.
2. **Their apps.** Call `status`. It shows their apps, or that they have
   none yet.
3. **The questions.** Ask at most four, in plain words: what the app
   should do; what it needs to see in their store; whether it should
   change anything; where they'll look for it.
4. **The plan.** Call `draft_plan` with their answers and ask whether it
   is right. If they want a change, draft it again.

Each tool's answer ends with what to do next. Follow it.
