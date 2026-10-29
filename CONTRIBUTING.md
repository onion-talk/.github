# Contributing to OnionTalk

Thank you for your interest in contributing to **OnionTalk** — the zero-knowledge, end-to-end encrypted P2P messenger over Tor v3 Hidden Services.

Every contribution that strengthens censorship resistance, cryptographic auditability, or the global volunteer .onion relay mesh helps protect private human communication worldwide.

---

## Ways to Contribute

### 1. Run a Volunteer Tor v3 Relay Node (oniontalk-relay)
The fastest way to strengthen the network is by spinning up a zero-knowledge store-and-forward relay node behind residential NAT, CGNAT, Raspberry Pi, or any Linux VPS using Docker:
- Repository: [onion-talk/oniontalk-relay](https://github.com/onion-talk/oniontalk-relay)
- No static IP, no port forwarding, and no domain/TLS certificate required.

### 2. Test the Android Demo APK & Report Compatibility (oniontalk-demo)
Help us test the pre-Play Store Android build across diverse devices and privacy-focused Android ROMs (**GrapheneOS**, **CalyxOS**, **LineageOS**, **DivestOS**, and standard Android 8.0+):
- Repository: [onion-talk/oniontalk-demo](https://github.com/onion-talk/oniontalk-demo)
- Report UI/UX feedback, Tor bootstrap timing, or SOCKS5/Orbot interoperability via GitHub Issues.

### 3. Cryptographic & Protocol Peer Review (oniontalk-protocol)
Review our wire format specification, threat model, and anti-forensic guarantees (X25519 + HKDF-SHA256 + ChaCha20-Poly1305, Auto-Gossip PEX, ACK Preimage Lock, and Synchronized Bilateral Burn):
- Repository: [onion-talk/oniontalk-protocol](https://github.com/onion-talk/oniontalk-protocol)

---

## Pull Request Guidelines

1. **Zero Metadata & Zero Telemetry**: Never introduce clearnet calls, analytics SDKs, DNS lookups outside SOCKS5h, or persistent logs containing IP/timing identifiers.
2. **Conventional Commits**: Use clear commit messages (eat:, ix:, docs:, security:, chore:).
3. **Security Disclosures**: If you discover a cryptographic or anonymity vulnerability, please follow [SECURITY.md](./SECURITY.md) rather than opening a public issue containing exploit details.
