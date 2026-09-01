# Kindle AI Quota Dashboard

A privacy-conscious dashboard that displays local AI service quota snapshots on a jailbroken Kindle.

The project separates local collection from the static e-ink page. It supports a private LAN deployment or a user-owned static host for Kindles that move between Wi-Fi networks.

All providers are disabled by default. Demo mode uses fake data and reads no credentials.
The Kindle page validates incoming snapshots, keeps a short-lived local cache for transient network failures, and marks fallback data as stale instead of presenting it as live.

```powershell
npm.cmd run demo
npm.cmd run build
npm.cmd run serve
```

Before enabling real providers or public hosting, read [SECURITY.md](SECURITY.md) and [docs/privacy.md](docs/privacy.md).

Version 0.1.1 is backward-compatible with the existing configuration format, four-card default layout, and Kindle entry point. Run `npm run check` after syncing an existing fork.

The project is not affiliated with Anthropic, OpenAI, Moonshot AI, DeepSeek, or Amazon. Product names are used only to describe compatibility.

Licensed under the [MIT License](LICENSE).
