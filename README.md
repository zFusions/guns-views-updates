# Guns Views

**Desktop control panel for guns.lol profile view campaigns.**

Free Windows app with a local backend, built-in proxy manager, campaign queue, and auto-updates. No Python or CLI setup required for end users.

---

## Download

| | |
|---|---|
| **Latest version** | **1.2.3** |
| **Installer** | [GunsViews-Setup-1.2.3.exe](https://github.com/zFusions/guns-views-updates/releases/latest/download/GunsViews-Setup-1.2.3.exe) |
| **All releases** | [github.com/zFusions/guns-views-updates/releases](https://github.com/zFusions/guns-views-updates/releases) |

> The desktop app checks this repository for updates. Each release ships `GunsViews-Setup-x.y.z.exe` and `latest.yml`.

---

## Install (Windows)

1. Download **GunsViews-Setup-1.2.3.exe** from [Releases](https://github.com/zFusions/guns-views-updates/releases/latest).
2. Run the installer and accept the Terms of Use.
3. Launch **Guns Views** from the Start Menu.
4. On first launch, wait for the setup screen (Turnstile solver + Camoufox warm-up).
5. Paste your proxies in the setup wizard, then launch a test campaign.

**Install location:** `%LOCALAPPDATA%\Programs\Guns Views`

---

## Quick start

1. **Proxies** â€” Add at least one working proxy (NodeProxies rotating gateway supported).
2. **Target** â€” Enter `guns.lol/username` or just the username.
3. **Views** â€” Set how many profile views to send.
4. **Speed** â€” Start with **Best** for the safest pace.
5. **Launch** â€” Click **Launch campaign** or queue multiple profiles.

---

## Proxy formats

One proxy per line:

```
host:port
host:port:user:pass
http://user:pass@host:port
np_xxx:password@eu-1.nodeproxies.xyz:8080
```

---

## Auto-update

- Open Guns Views â†’ **Check for updates** in the footer, or wait a few seconds after launch.
- When a new version is available, download and install from this repository automatically.
- Updates install into the same folder as the running app.

---

## Requirements

| | |
|---|---|
| OS | Windows 10/11 (64-bit) |
| Proxies | Required for campaigns |
| Internet | Required for guns.lol + update checks |
| Python / Node / Go | **Not required** (bundled in the installer) |

---

## Troubleshooting

| Issue | Fix |
|-------|-----|
| Stuck on old version after install | Uninstall, delete `%LOCALAPPDATA%\Programs\Guns Views`, reinstall from latest release |
| Wrong version shown in footer | Hover the version â€” check install path is `%LOCALAPPDATA%\Programs\Guns Views` |
| Update fails | See `%TEMP%\guns-views-update.log` |
| App â€œclosesâ€ when clicking X | It minimizes to the system tray â€” right-click tray icon â†’ **Quit** |

---

## Whatâ€™s included

- Local Go backend + embedded desktop UI
- Free Turnstile solver (Zkamo + Camoufox) â€” no paid captcha API
- Proxy health checks and campaign queue
- English / French UI
- Discord webhooks (optional)
- Background mode via system tray

---

## Repository purpose

This repository hosts **public release files only** for the Guns Views desktop updater:

- `GunsViews-Setup-<version>.exe` â€” Windows installer
- `latest.yml` â€” Update manifest (version + SHA-512)

Source code is maintained separately and is not published here.

---

## Credits

Open-source components used by Guns Views:

- [Zkamo/turnstile-solver](https://github.com/Zkamo/turnstile-solver) â€” local Turnstile solver
- [CuteTenshii/guns-solver](https://github.com/CuteTenshii/guns-solver) â€” PoW / analytics format
- [glockinhand/guns.lol-view-bot](https://github.com/glockinhand/guns.lol-view-bot) â€” transport tuning

---

**Guns Views** Â· Free desktop app Â· Updates via this repository
