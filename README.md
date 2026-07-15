<p align="center">
  <img src="https://raw.githubusercontent.com/zFusions/guns-views-updates/main/github_assets/logo.png" alt="Guns Views" width="96" />
</p>

<h1 align="center">Guns Views</h1>

<p align="center">
  <strong>Desktop control panel for guns.lol profile view campaigns</strong><br />
  Free Windows app | local backend | proxy manager | campaign queue | auto-updates
</p>

<p align="center">
  <a href="https://github.com/zFusions/guns-views-updates/releases/latest">Download latest</a>
  |
  <a href="#install-windows">Install guide</a>
  |
  <a href="#quick-start">Quick start</a>
  |
  <a href="#troubleshooting">Troubleshooting</a>
</p>

---

## Download

| | |
|---|---|
| **Latest version** | **1.4.14** |
| **Installer** | [GunsViews-Setup-1.4.14.exe](https://github.com/zFusions/guns-views-updates/releases/latest/download/GunsViews-Setup-1.4.14.exe) |
| **All releases** | [github.com/zFusions/guns-views-updates/releases](https://github.com/zFusions/guns-views-updates/releases) |

> The desktop app checks this repository for updates. Each release ships `GunsViews-Setup-x.y.z.exe` and `latest.yml`.

---

## Recommended proxies

<p align="center">
  <a href="https://nodeproxies.xyz/register?ref=C8395E27">
    <img src="https://nodeproxies.xyz/standard.gif" alt="NodeProxies - residential rotating proxies" width="720" />
  </a>
</p>

> **NodeProxies** is the recommended proxy provider for Guns Views campaigns.
>
> Rotating residential gateways work out of the box with the built-in proxy manager and health checks.
>
> **Official referral link:** [nodeproxies.xyz/register?ref=C8395E27](https://nodeproxies.xyz/register?ref=C8395E27)

| | NodeProxies |
|---|---|
| **Type** | Residential rotating proxies |
| **Use case** | guns.lol view campaigns with proxy rotation |
| **Format** | `np_xxx:password@eu-1.nodeproxies.xyz:8080` |
| **Register** | [nodeproxies.xyz/register?ref=C8395E27](https://nodeproxies.xyz/register?ref=C8395E27) |

---

## Install (Windows)

1. Download **GunsViews-Setup-1.4.14.exe** from [Releases](https://github.com/zFusions/guns-views-updates/releases/latest).
2. Run the installer and accept the Terms of Use.
3. Launch **Guns Views** from the Start Menu.
4. On first launch, wait for the setup screen (Turnstile solver + Camoufox warm-up).
5. Paste your proxies in the setup wizard, then launch a test campaign.

**Install location:** `%LOCALAPPDATA%\Programs\Guns Views`

**User data (settings, proxies, presets):** `%LOCALAPPDATA%\Guns Views\Data`

> Updates keep your settings and proxy list. User data is stored outside the install folder.

---

## Quick start

1. **Proxies** - Add at least one working proxy ([NodeProxies](https://nodeproxies.xyz/register?ref=C8395E27) rotating gateway supported).
2. **Target** - Enter `guns.lol/username` or just the username.
3. **Views** - Set how many profile views to send.
4. **Speed** - Start with **Best** for the safest pace.
5. **Launch** - Click **Launch campaign** or queue multiple profiles.

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

- Open Guns Views -> **Check for updates** in the sidebar, or wait a few seconds after launch.
- When a new version is available, download and install from this repository automatically.
- Updates install into the same folder as the running app.
- **Your proxies, presets, and settings are preserved** in `%LOCALAPPDATA%\Guns Views\Data`.

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
| Wrong version shown in footer | Hover the version - check install path is `%LOCALAPPDATA%\Programs\Guns Views` |
| Config lost after update | Upgrade to **1.4.14** or newer - data is stored in `%LOCALAPPDATA%\Guns Views\Data` |
| Update fails | See `%TEMP%\guns-views-update.log` |
| App "closes" when clicking X | It minimizes to the system tray - right-click tray icon -> **Quit** |

---

## What's included

- Local Go backend + embedded desktop UI
- Free Turnstile solver (Zkamo + Camoufox) - no paid captcha API
- Proxy health checks and campaign queue
- English / French UI
- Discord webhooks (optional)
- Background mode via system tray

---

## Repository purpose

This repository hosts **public release files only** for the Guns Views desktop updater:

- `GunsViews-Setup-x.y.z.exe` - Windows installer
- `latest.yml` - Update manifest (version + SHA-512)

Source code is maintained separately and is not published here.

---

## Disclaimer

> **IMPORTANT - READ BEFORE USE**
>
> Guns Views is provided **free of charge** and **as-is**, without warranty of any kind.
>
> The author **strictly and absolutely disclaims all liability** for any direct or indirect damage, loss of account, suspension, ban, data loss, legal issue, or misuse arising from the use of this software.
>
> You are solely responsible for how you use Guns Views, which proxies you use, and compliance with guns.lol terms of service and applicable laws.
>
> This project is intended for **educational and personal use**. Proceed at your own risk.

---

## Credits

Open-source components used by Guns Views:

- [Zkamo/turnstile-solver](https://github.com/Zkamo/turnstile-solver) - local Turnstile solver
- [CuteTenshii/guns-solver](https://github.com/CuteTenshii/guns-solver) - PoW / analytics format
- [glockinhand/guns.lol-view-bot](https://github.com/glockinhand/guns.lol-view-bot) - transport tuning

---

<p align="center">
  <strong>Guns Views</strong> | Free desktop app | Updates via this repository
</p>
