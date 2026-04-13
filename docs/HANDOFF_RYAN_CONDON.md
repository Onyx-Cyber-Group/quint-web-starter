# Handoff — Ryan Condron (web frontend)

Welcome. This repo is intentionally **small**: one HTML page, vanilla JS, Vite for dev proxy + build.

## Your mission

Grow this into the **Splash MMP web client** (or adjacent tools) consuming the same backend as iOS:

- **Base host (POC):** `https://100.25.66.46` — Synapse + Quint API adapter on one host.
- **Auth:** Matrix user `access_token` as `Authorization: Bearer …` for protected REST routes.
- **Docs:** skim `quint-messaging-server/api/openapi/` and server `README` files; iOS `APIConfiguration.swift` lists canonical paths.

## Day-1 checklist

1. Clone repo, `npm install`, `npm run dev`.
2. Confirm **Health** and **AI status** buttons return JSON.
3. Obtain a **test Matrix account** from Onyx; log in via `/_matrix/client/v3/login`; paste `access_token` into the third panel; confirm **whoami** succeeds.
4. Read the main **README.md** section on credentials and TLS.

## Security

- Never commit **tokens, passwords, or `.pem` keys**.
- Do not embed **admin** tokens in the browser.
- Treat pasted tokens in the starter UI as **volatile** (clear after session).

## Questions

Ping **Cpt. Sadat** / ONYX engineering on Slack `#quint-radio` or your onboarding channel.
