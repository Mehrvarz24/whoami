# WhoAmI — Browser Fingerprint & Privacy Score

Live demo: **https://mehrvarz24.github.io/whoami-fingerprint/**

Also running at: https://whoami.miors.art

A single-page tool (in the spirit of browserleaks.com) that shows what your browser leaks:

- IP address, country/city/postal/coordinates, ISP, ASN, VPN/proxy detection
- Device type, CPU cores, RAM, GPU renderer, battery, touch support
- Browser/OS, language, timezone vs IP timezone mismatch
- WebRTC real-IP leak (STUN), canvas fingerprint hash, Do-Not-Track
- **0–100 privacy risk score** with per-factor breakdown — flags VPN/proxy usage via timezone, language and ISP heuristics

No build step, no dependencies — pure HTML/CSS/JS. The GitHub Pages version is fully client-side (IP info fetched from ipwho.is). The server version (whoami.miors.art) adds server-side scoring via `server.py` (Python stdlib only).
