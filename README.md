# BPB VPN Desktop

**A flexible Windows VPN client built on the BPB project.**

BPB VPN Desktop brings BPB's proxy and tunnelling capabilities to Windows through a native desktop interface, with installer and portable distributions.

> BPB is a networking tool, not a guarantee of access or anonymity. Availability and connection quality depend on your network, server, configuration and local restrictions.

## Features

- VLESS / Cloudflare Workers connections.
- WARP (WireGuard) and MASQUE support.
- BPB and Aether core integration with separate core selection.
- Alternative WARP/MASQUE registration methods and endpoint discovery.
- Cloudflare and Aether endpoint scanners.
- SSH, Tor, Psiphon and Serverless connection options.
- Tor bridge retrieval, custom bridge management and bridge testing.
- Exit-node selection, proxy chaining and region selection.
- Advanced DNS options: Local DNS, Anti-Sanctions DNS and Fake DNS.
- IPv6, MTU and LAN proxy sharing controls.
- Routing presets for Iran, China and Russia, plus custom bypass, sanction and block rules.
- In-app GeoIP and GeoSite asset updates.
- Browser security features, including WebRTC leak protection and browser privacy guidance.
- Companion browser extensions for Firefox and Microsoft Edge.
- Live upload/download traffic and Worker Request usage statistics.
- Public IP, Cloudflare IP, ping and connection-duration information.
- Windows system-tray integration and in-app release update checking.
- Light/dark/system themes, accent colors and adjustable font size.
- Built-in fonts and support for custom TTF/OTF fonts.
- Settings import, export and sharing.

Availability of individual protocols and options can vary with the selected connection type and bundled core version.

## Geo routing by country

Choose one country in **Settings → Routing → Bypass rules**: Iran (the default), China or Russia. The app keeps one active `geoip.dat` / `geosite.dat` pair in its assets and automatically selects the appropriate download source for the country you chose when you use **Update Geo**.

- **Iran:** [Chocolate4U/Iran-v2ray-rules](https://github.com/Chocolate4U/Iran-v2ray-rules) — GeoIP and GeoSite.
- **China:** [Loyalsoldier/v2ray-rules-dat](https://github.com/Loyalsoldier/v2ray-rules-dat) — GeoIP and GeoSite.
- **Russia:** GeoIP from [Loyalsoldier/v2ray-rules-dat](https://github.com/Loyalsoldier/v2ray-rules-dat) (for the `geoip:ru` country tag), and GeoSite from [runetfreedom/russia-v2ray-rules-dat](https://github.com/runetfreedom/russia-v2ray-rules-dat) (for Russia-specific domain categories).

**Important:** After changing the selected country, you must run **Update Geo** once before relying on country-based routing. Until the matching files have been downloaded and verified, Geo-based routing rules are held back so the previous country's files are not used by mistake. Your custom domain/IP rules and the independent BitTorrent switch remain separate.

## Download

Get the latest Windows release from the [Releases page](https://github.com/NottDevv/BPB-VPN-Desktop/releases/latest).

- **Setup** — the standard Windows installer.
- **Portable** — the application bundle, which can run without a conventional installation.

## Browser extensions

Companion extensions are available for supported browsers. Visit the [development repository](https://github.com/NottDevv/BPB-VPN-Desktop-Dev) for their source and installation information.

## Project repositories

- **Releases and downloads:** [NottDevv/BPB-VPN-Desktop](https://github.com/NottDevv/BPB-VPN-Desktop)
- **Source code and development:** [NottDevv/BPB-VPN-Desktop-Dev](https://github.com/NottDevv/BPB-VPN-Desktop-Dev)

## Credits and license

BPB VPN Desktop is based on the BPB project and its open-source ecosystem. Please refer to the source repository's [LICENSE](https://github.com/NottDevv/BPB-VPN-Desktop-Dev/blob/desktop/bootstrap/LICENSE) and the licenses/notices shipped with bundled third-party components for the applicable terms.

For bug reports, feature requests and source-level discussion, use the [development repository](https://github.com/NottDevv/BPB-VPN-Desktop-Dev/issues).
