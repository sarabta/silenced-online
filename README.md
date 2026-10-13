# Silenced Online

Y+ (yplus.ps) interactive simulation, story 3 of the Communicating Palestine toolkit.
Live at: https://silenced.yplus.ps/

- `index.html`: the interactive
- `silenced-online-data.json`: all copy in EN / IT / FR / AR, countries, cases, sources, evidence figures
- `support.js`: runtime
- `assets/yplus-logo.png`

URL parameters: `?lang=en|it|fr|ar`, `?mode=kiosk` (90 s idle reset, nothing stored).

Privacy: name and post text never leave the browser. GA4 (G-NMEYZ7ZWB5) events use the `silenced_` prefix and never include name or post text.

Deploy: every push to main rsyncs the repo to the server via .github/workflows/deploy.yml. Required secrets: SSH_PRIVATE_KEY, SSH_HOST, SSH_PORT, SSH_USER, TARGET_PATH.
