# Security Policy

## Zero-Knowledge Architecture & Threat Model

OnionTalk is engineered under a strict Zero-Trust / Zero-Knowledge threat model:

- All client-to-relay and relay-to-relay traffic traverses **Tor v3 Hidden Services** (`SOCKS5h`).
- Payloads are encrypted end-to-end on the client device (`X25519` + `HKDF-SHA256` + `ChaCha20-Poly1305`) and wrapped in an `AES-256-GCM` transport cipher.
- Relay nodes store only encrypted envelopes and purge them upon verifying the cryptographic preimage `SHA-256(ack_token) == ack_hash`.

## Reporting a Vulnerability

If you discover a cryptographic flaw, deanonymization vector, or denial-of-service vulnerability in the OnionTalk protocol or relay implementation:

1. **Do not open a public GitHub issue** for unpatched security vulnerabilities.
2. Report the finding via [GitHub Private Vulnerability Reporting](https://github.com/onion-talk/oniontalk-relay/security/advisories/new) or contact the security team directly via `security@oniontalk.org`.
3. Include a minimal reproduction script or proof-of-concept and the affected component (`oniontalk-relay`, `oniontalk-protocol`, or client).
