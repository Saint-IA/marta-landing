# marta-landing

Public landing page for the MARTA lead intake chat widget.

## What this is

Static single-page site (`public/index.html`) hosting an embedded chat
widget that posts to a private n8n backend over a Cloudflare Tunnel.
No build step, no framework, vanilla JS.

## Where it deploys

Cloudflare Workers Static Assets, auto-deployed on every push to `main`
via Workers Builds (Cloudflare's native Git CI). Custom domain configured
in the Cloudflare dashboard.

## How to update

Edit `public/index.html`, commit, push to `main`. Workers Builds picks
up the change and deploys within ~30 seconds. Rollbacks available from
the Cloudflare dashboard if needed.