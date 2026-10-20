<div align="center">
  <img src="https://raw.githubusercontent.com/onion-talk/.github/main/assets/oniontalk-icon-512.png" alt="OnionTalk Logo" width="130" height="130" />
  <h1>OnionTalk</h1>
  <p><strong>Zero-Knowledge, End-to-End Encrypted P2P Mesh Messenger over Tor v3 Hidden Services</strong></p>

  <p>
    <a href="https://play.google.com/store/apps/details?id=org.oniontalk.messenger">
      <img src="https://img.shields.io/badge/Google_Play-OnionTalk_–_Apps_no_Google_Play-3DDC84?style=for-the-badge&logo=google-play&logoColor=black" alt="OnionTalk – Apps no Google Play" />
    </a>
    <a href="https://github.com/sponsors/eriktonon">
      <img src="https://img.shields.io/badge/Sponsor-OnionTalk-ea4aaa?style=for-the-badge&logo=githubsponsors&logoColor=white" alt="Sponsor on GitHub" />
    </a>
    <a href="#-sponsor--donate">
      <img src="https://img.shields.io/badge/Donate-Bitcoin-F7931A?style=for-the-badge&logo=bitcoin&logoColor=white" alt="Donate Bitcoin" />
    </a>
    <a href="#-sponsor--donate">
      <img src="https://img.shields.io/badge/Donate-Ethereum-627EEA?style=for-the-badge&logo=ethereum&logoColor=white" alt="Donate Ethereum" />
    </a>
    <a href="#-sponsor--donate">
      <img src="https://img.shields.io/badge/Donate-Solana-14F195?style=for-the-badge&logo=solana&logoColor=black" alt="Donate Solana" />
    </a>
  </p>

  <p>
    <img src="https://img.shields.io/badge/Network-Tor_v3_Hidden_Services-7D4698?style=flat-square&logo=torproject&logoColor=white" alt="Tor v3" />
    <img src="https://img.shields.io/badge/E2EE-X25519_%2B_ChaCha20--Poly1305-00C853?style=flat-square" alt="E2EE" />
    <img src="https://img.shields.io/badge/Discovery-Auto--Gossip_PEX-1F6FEB?style=flat-square" alt="PEX" />
    <img src="https://img.shields.io/badge/Storage-Zero--Knowledge_Store--and--Forward-FF6D00?style=flat-square" alt="Zero Knowledge" />
  </p>
</div>

---

## 🎯 Our Mission

Most encrypted messengers protect message content while still exposing your social graph. They require a phone number to register, rely on centralized DNS-resolved servers, and log who talks to whom, when, and from which IP address. When a single jurisdiction orders a takedown or blocks an ASN, the entire network goes dark.

**Our mission is to make private human communication unstoppable and metadata-free.**

OnionTalk eliminates central servers, phone numbers, and clearnet IP exposure:

1. **Zero Identity Registration (256-bit Public Key ID)**: Your identity (`@<64-hex-ed25519-pubkey>:<domain>.onion`) embeds a full 256-bit **Ed25519** public key generated locally on your device and birationally mapped to **X25519**. No phone number, email, or central account server exists.
2. **100% Tor v3 Hidden Service Transport**: Every client and relay communicates exclusively through 56-character `.onion` v3 addresses over SOCKS5h (`127.0.0.1:9050`). Neither the sender, the recipient, nor the relay node ever learns another participant's IP address or physical location.
3. **Zero-Knowledge RAM-Only Federated Mesh**: Every message is sealed with a fresh ephemeral **X25519** keypair (`Ephemeral-Static + Static-Static ECDH` + `HKDF-SHA256` + `ChaCha20-Poly1305 AEAD`) and signed with the sender's **Ed25519** private key (`__ENC_X25519_CHACHA20_V2__`). Relays hold messages strictly in volatile RAM (`ram-volatile-ephemeral-ttl24h`), enforce **Ed25519** signature authentication on `/inbox` and `/ack`, and require a CSPRNG 256-bit preimage proof (`SHA-256(ack_token) == ack_lock`) before purging envelopes.
4. **Censorship Immunity by Design**: Anyone can spin up a relay node behind residential NAT or CGNAT with a single Docker command. Through Ed25519-authenticated Peer Exchange (`Auto-Gossip PEX`) and epidemic gossip fanout, every new node strengthens the mesh without requiring port forwarding, static IPs, or TLS certificates.

---

## 📱 Official Release on Google Play & Live Walkthrough ("Pablo & Bruna")

> 🚀 **Available Now on Google Play Store**: Download the official OnionTalk Android application directly on Google Play: [**OnionTalk – Apps no Google Play**](https://play.google.com/store/apps/details?id=org.oniontalk.messenger).

Below is a real-time demonstration captured from two independent Android emulators (**Pablo** and **Bruna**) conversing in English over the OnionTalk Tor v3 mesh—with zero SIM card, zero phone number, and full anti-forensic local storage (`SQLCipher AES-256-CBC` + `Argon2id`).

👉 **[Download on Google Play (`org.oniontalk.messenger`) →](https://play.google.com/store/apps/details?id=org.oniontalk.messenger)**  
👉 **[Explore the Full Screen-by-Screen Technical Walkthrough (`oniontalk-demo`) →](https://github.com/onion-talk/oniontalk-demo)**

<div align="center">
  <a href="https://github.com/onion-talk/oniontalk-demo/raw/main/video/OnionTalk-Freedom-EN.mp4">
    <img src="https://raw.githubusercontent.com/onion-talk/oniontalk-demo/main/video/poster-freedom.png" width="820" alt="Watch OnionTalk Official Promo Video" />
  </a>
  <br /><br />
  <a href="https://github.com/onion-talk/oniontalk-demo/raw/main/video/OnionTalk-Freedom-EN.mp4">
    <img src="https://img.shields.io/badge/%E2%96%B6_Watch_Promo_Video_(English)-1080p_MP4-00E5FF?style=for-the-badge&logoColor=black" alt="Watch Promo Video in English" />
  </a>
  <a href="https://github.com/onion-talk/oniontalk-demo/raw/main/video/OnionTalk-Liberdade-PT.mp4">
    <img src="https://img.shields.io/badge/%E2%96%B6_Assistir_V%C3%ADdeo_(Portugu%C3%AAs)-1080p_MP4-00E676?style=for-the-badge&logoColor=black" alt="Assistir Vídeo em Português" />
  </a>
</div>
<br />

| **1. Zero-PII Identity Creation (`Pablo`)** | **2. Pablo's View (Tor v3 E2EE Chat)** | **3. Bruna's View (Mirrored P2P Delivery)** |
| :---: | :---: | :---: |
| <img src="https://raw.githubusercontent.com/onion-talk/.github/main/assets/screenshots/02-create-identity-en.png" width="260" alt="Create Anonymous Account" /> | <img src="https://raw.githubusercontent.com/onion-talk/.github/main/assets/screenshots/04-chat-pablo-bruna-en.png" width="260" alt="Pablo Chat with Bruna" /> | <img src="https://raw.githubusercontent.com/onion-talk/.github/main/assets/screenshots/05-chat-bruna-pablo-en.png" width="260" alt="Bruna Chat with Pablo" /> |
| *Local Ed25519/X25519 key generation & Argon2id vault without phone numbers or emails.* | *Pablo chatting with Bruna in Lisbon over `.onion` relays with zero roaming or IP tracking.* | *Bruna receiving and replying to Pablo's encrypted payloads in real time.* |

| **4. Synchronized Bilateral Burn (`🔥`)** | **5. Federated `.onion` Mesh & Tor SOCKS5h** | **6. SQLCipher AES-256 & Anti-Forensics** |
| :---: | :---: | :---: |
| <img src="https://raw.githubusercontent.com/onion-talk/.github/main/assets/screenshots/06b-after-synchronized-burn-en.png" width="260" alt="Synchronized Burn Scrambled Chat" /> | <img src="https://raw.githubusercontent.com/onion-talk/.github/main/assets/screenshots/08-tor-mesh-settings-en.png" width="260" alt="Tor Mesh Settings" /> | <img src="https://raw.githubusercontent.com/onion-talk/.github/main/assets/screenshots/09-security-sqlcipher-en.png" width="260" alt="SQLCipher Security Audit" /> |
| *In-place B-Tree cell overwrite with cryptographic noise (`🔥`) on both devices simultaneously.* | *9 active `.onion` v3 relays discovered via `Auto-Gossip PEX` over `127.0.0.1:9050`.* | *`FLAG_SECURE`, 5-strike duress wipe, zero-FCM local Tor push, and manual `VACUUM`.* |

---

## 📦 Organization Repositories

This organization follows a modular structure for the OnionTalk protocol, relay infrastructure, and application demo:

| Repository | Role | Stack | Status |
| :--- | :--- | :--- | :--- |
| [**`oniontalk-demo`**](https://github.com/onion-talk/oniontalk-demo) | Official Google Play App Link & Step-by-Step Visual Walkthrough (*Pablo & Bruna* Dual-Emulator Demo) | Android, SQLCipher, Tor v3, Documentation | ![Active](https://img.shields.io/badge/Google_Play-available-00C853?style=flat-square) |
| [**`oniontalk-relay`**](https://github.com/onion-talk/oniontalk-relay) | Zero-Knowledge Tor v3 Hidden Service Relay Node with Ed25519-Authenticated Gossip PEX, RAM-Only Volatile Queues, and Cryptographic ACK Preimage Lock | Python 3.12, Flask, Gunicorn, Cryptography, Tor v3, Docker Compose | ![Active](https://img.shields.io/badge/status-production-00C853?style=flat-square) |
| [**`oniontalk-protocol`**](https://github.com/onion-talk/oniontalk-protocol) | OnionTalk Wire Protocol Specification, 4-Layer Cryptographic Stack, Epidemic Gossip Routing, and Anti-Censorship Manifesto | Markdown, Mermaid, Cryptographic Specs | ![Active](https://img.shields.io/badge/status-stable-1F6FEB?style=flat-square) |
| [**`.github`**](https://github.com/onion-talk/.github) | Organization Profile, Community Health Files, Security Disclosure Policy, and Funding Configuration | GitHub Actions, YAML, Markdown | ![Active](https://img.shields.io/badge/status-active-00C853?style=flat-square) |

---

## 🏗️ Protocol Architecture at a Glance

| Layer | Technology | Security Guarantee |
| :--- | :--- | :--- |
| **L1: Anonymity & Routing** | Tor v3 Hidden Services (`SOCKS5h`, Ed25519 56-char `.onion`, `127.0.0.1` local bind) | Conceals IP addresses of senders, recipients, and relays. Works behind CGNAT without open router ports. |
| **L2: Service Discovery** | Bootstrap Seeds + Ed25519-Authenticated Peer Exchange (`Auto-Gossip PEX`) | Relays sign peer announcements with Ed25519 and verify `node_pubkey` over Tor (`/health`) before admitting peers. |
| **L3: Epidemic Gossip & Storage** | RAM-Only Volatile Store-and-Forward (`24h TTL`) + Ed25519 Inbox Auth + ACK Lock | Envelopes reside strictly in RAM, require Ed25519 challenge signatures on `/inbox`, and purge upon verifying `SHA-256(ack_token) == ack_lock`. |
| **L4: End-to-End Encryption** | `X25519` (Ephemeral+Static ECDH) + `HKDF-SHA256` + `ChaCha20-Poly1305` + `Ed25519` Signature | Per-message forward secrecy and sender authenticity on the client device; local storage protected by `SQLCipher AES-256-CBC` + `Argon2id`. |

---

## 🚀 Run a Relay Node in 60 Seconds

You can join the global OnionTalk federated mesh from any Linux server, VPS, Raspberry Pi, or home machine behind CGNAT. No port forwarding or domain name is required:

```bash
git clone https://github.com/onion-talk/oniontalk-relay.git
cd oniontalk-relay
docker compose up -d --build
```

Verify your node's `.onion` v3 address and mesh synchronization status:

```bash
curl http://localhost:8080/health
```

---

## 💖 Sponsor & Donate

OnionTalk is an independent open-source project with zero venture capital, zero ads, and zero user data monetization. Community contributions directly fund dedicated Tor v3 seed relays, multi-region bandwidth, and independent cryptographic audits.

<p align="center">
  <a href="https://github.com/sponsors/eriktonon">
    <img src="https://img.shields.io/badge/💙_Sponsor_via_GitHub_Sponsors-ea4aaa?style=for-the-badge&logo=githubsponsors&logoColor=white" alt="GitHub Sponsors" />
  </a>
</p>

### Direct Cryptocurrency Donations

| Network | Wallet Address |
| :--- | :--- |
| **Bitcoin (`BTC`)** | `bc1q0hr95ay33rtazfepg64yddf52q3yqh7ud83cza` |
| **Ethereum (`ETH`)** | `0xE69FCE4Fa35CF3bd98F496337b1eA223270b2c92` |
| **Solana (`SOL`)** | `3E8L1Hdqe7Xk6GCrzHbtY5sReAfLFc9CdwgZxP7qaoHq` |
