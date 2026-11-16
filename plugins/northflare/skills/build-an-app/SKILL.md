---
name: build-an-app
description: Build a custom Shopify app with Northflare. Use when the person wants a custom app for their Shopify store, or asks about their Northflare apps.
---

# Building a Shopify app with Northflare

Northflare builds and hosts custom Shopify apps for store owners, most of
whom are not developers. Its tools come from the Northflare connector that
this plugin adds.

1. **Their apps.** Call `status`. It shows their apps, or that they have
   none yet.
2. **Sign in, if asked.** If a Northflare tool answers that the person
   needs to sign in, their app is showing them a button for it: in
   Codex, **Reconnect** on a banner. Ask them to press it and sign in on
   Northflare's page, then call the tool again. Only they sign in; never
   ask them to type a command in a terminal. If Northflare's tools aren't
   in this conversation at all, they arrive in a new one: in Codex, offer
   to open it for them with `create_thread`.
3. **The questions.** Ask at most four, in plain words: what the app
   should do; what it needs to see in their store; whether it should
   change anything; where they'll look for it.
4. **The plan.** Call `draft_plan` with their answers and ask whether it
   is right. If they want a change, draft it again.

Each tool's answer ends with what to do next. Follow it.
