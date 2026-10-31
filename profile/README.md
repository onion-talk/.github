<div align="center">
  <img src="https://raw.githubusercontent.com/onion-talk/.github/main/assets/oniontalk-icon-512.png" alt="OnionTalk Logo" width="130" height="130" />
  <h1>OnionTalk</h1>
  <p><strong>Zero-Knowledge, End-to-End Encrypted P2P Mesh Messenger over Tor v3 Hidden Services</strong></p>

  <p>
    <a href="https://play.google.com/store/apps/details?id=org.oniontalk.messenger">
      <img src="https://img.shields.io/badge/Google_Play-OnionTalk_–_Apps_no_Google_Play-3DDC84?style=for-the-badge&logo=google-play&logoColor=black" alt="OnionTalk – Apps no Google Play" />
    </a>
    <a href="https://github.com/onion-talk/oniontalk-demo/releases/download/v1.5.4/OnionTalk-v1.5.4.apk">
      <img src="https://img.shields.io/badge/Direct_APK-OnionTalk_v1.5.4_(Build_48)-00E5FF?style=for-the-badge&logo=android&logoColor=black" alt="Download OnionTalk v1.4.2 Build 22 APK" />
    </a>
    <a href="https://github.com/onion-talk/oniontalk-relay/releases/download/v1.5.2/OnionTalk-RelayNode-v1.5.2.apk">
      <img src="https://img.shields.io/badge/Relay_APK-Relay_Node_v1.5.2_(Build_11_Zero--Leak)-00E676?style=for-the-badge&logo=torproject&logoColor=black" alt="Download OnionTalk Relay Node v1.0.1 Zero-Leak APK" />
    </a>
    <a href="https://hub.docker.com/r/eriktonon/oniontalk-web">
      <img src="https://img.shields.io/badge/Docker_Web_Client-eriktonon%2Foniontalk--web:latest-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker Hub OnionTalk Web Client & Relay" />
    </a>
    <a href="#-sponsor--donate">
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
    <img src="https://img.shields.io/badge/PQC_E2EE-X25519_%2B_ML--KEM--768_%2B_ChaCha20-00C853?style=flat-square" alt="E2EE" />
    <img src="https://img.shields.io/badge/Discovery-Auto--Gossip_PEX-1F6FEB?style=flat-square" alt="PEX" />
    <img src="https://img.shields.io/badge/Storage-Zero--Knowledge_Store--and--Forward-FF6D00?style=flat-square" alt="Zero Knowledge" />
  </p>
</div>

---

## 🚀 What's New in `v1.5.4` (`versionCode = 48` / Build 48) & Relay Node `v1.5.2` (`Build 11`) & Mesh `v=31` — Sovereign PQC Groups, In-RAM Image Blur Studio, Post-Quantum Hybrid Encryption (`ML-KEM-768`), Dual Warm Socket Pool (`~1.13s` E2E) & 20-Node Zero-Leak Mesh

- **📦 Direct Signed APK Downloads & Web Container (`v1.5.4` — Latest Release Build 48)**:
  - **Main Messenger APK (`org.oniontalk.messenger` `v1.5.4` Build 48)**: [**Download `OnionTalk-v1.5.4.apk`**](https://github.com/onion-talk/oniontalk-demo/releases/download/v1.5.4/OnionTalk-v1.5.4.apk) (`SHA-256: 91c089e10a8ca1ab0326b87d66fff9e29d90797c03921d4e5bfc586d9b86c34a`)
  - **Standalone Android Relay Node APK (`org.oniontalk.relaynode` `v1.5.2` Build 11)**: [**Download `OnionTalk-RelayNode-v1.5.2.apk`**](https://github.com/onion-talk/oniontalk-relay/releases/download/v1.5.2/OnionTalk-RelayNode-v1.5.2.apk) (`SHA-256: eac1ccbe461eabb9f42a6485628c0d9b3cce0f378ba217572a1beba975c5279c`)
  - **🐳 Desktop & Web Container + Embedded Tor v3 Relay (`Windows / Linux / macOS`)**: [**`eriktonon/oniontalk-web:latest`**](https://hub.docker.com/r/eriktonon/oniontalk-web) (`v1.5.4-build48` — `sha256:f0f2912ef2c675f29f30d3f6cb7259b2724b435ab37208f20bc23a86e676d1b1`) — Self-contained Rust Black-Box Web Messenger + active Tor v3 Hidden Service Relay listening on `127.0.0.1:8420`.

- **🛡️ Key Cryptographic & P2P Mesh Breakthroughs in `v1.5.4` (`Build 48` & Relay `Build 10`)**:
  1. **Sovereign Post-Quantum Encrypted Groups (`PQC Groups`) & Anti-Spam Proof-of-Community**: End-to-end encrypted multi-party group chats over Tor v3 with zero central member servers. Group creation unlocks automatically via organic local proof-of-community (`3+ mutual contacts` + `5+ days of vault maturity`, evaluated 100% locally) or immediately via an offline `Ed25519`-signed **`FounderPass`** certificate granted to community Relay Node Operators (`2+ hours active uptime`) or voluntary crypto supporters.
  2. **In-RAM Image Blur & Pixelation Studio + Zero-EXIF Sanitizer**: Built-in tactile brush editor (`Gaussian Blur` & `Mosaic Pixelate`) operating strictly in volatile RAM before encryption, combined with 100% EXIF/GPS header stripping and Least Significant Bit (`LSB`) anti-fingerprinting jitter.
  3. **Hybrid Post-Quantum Cryptography (`__ENC_PQC_KYBER768_X25519_V3__`)**: Combines classical **Dual X25519 ECDH** with **NIST FIPS 203 ML-KEM-768 (`Kyber-768`)** key encapsulation via `HKDF-SHA256` + `ChaCha20-Poly1305 AEAD` + `Ed25519` outer envelope signatures to protect against *Harvest Now, Decrypt Later* quantum adversaries.
  4. **Ultra-Fast E2E Delivery (`1.139s – 1.244s`, avg `1.20s`)**: Upgraded **Dual Warm Socket Pool** (`minWarmSockets = 2` per `.onion` gateway, `70s/75s` Keep-Alive) achieving **100% pre-warmed Tor circuit reuse (`0ms` SOCKS5 handshake)** alongside a `250ms` speculative *Hedged Send*.
  5. **20-Node Zero-Leak Global Mesh (`v=31`), S/Kademlia XOR Distance Routing & Blinded Poller Affinity**: All **20 global `.onion` v3 relays** route by XOR distance (`SHA-256(peer_onion) ^ SHA-256(recipient_hash)`) with zero-knowledge RAM-only rendezvous affinity (`active_pollers`, `TTL 90s`, zero logs) and **100% anonymized synthetic node coordinates (Zero IP / Zero Cloud Provider Exposure)**.
  6. **GossipSub v1.2 `IHAVE` / `IDONTWANT` Deduplication & Mandatory `SHA-256` Media Integrity**: Relays announce `POST /gossip/ihave` metadata before forwarding payloads `> 1024 bytes` (cutting redundant Tor mesh bandwidth by **~70%**) and verify `SHA-256` Merkle hashes on all voice notes, images, and attachments prior to rendering.
---
## 🚀 What's New in `v1.4.2` (`versionCode = 18` / Internal `vc17`) — Password-Locked Messages & Chats, Unified Long-Press Menu, Profile Photo Privacy, 15s Auto-Lock & Official Video Suite

- **📦 Direct Signed APK Downloads (`v1.4.2` — Latest Fixed Build 18)**:
  - **Main Messenger APK (`org.oniontalk.messenger` `v1.4.2` Build 18)**: [**Download `OnionTalk-v1.5.4.apk`**](https://github.com/onion-talk/oniontalk-demo/releases/download/v1.5.4/OnionTalk-v1.5.4.apk) (`SHA-256: 68f3d5785919acaf0820c238f93f5db0cb02df5986db457ec783d573dbc652a8`)
  - **Release Build 18 APK (`versionCode = 18`)**: [**Download `OnionTalk-v1.4.1-b18-release.apk`**](https://github.com/onion-talk/oniontalk-demo/releases/download/v1.5.4/OnionTalk-v1.5.4.apk)
  - **Internal Test Track Build 17 APK (`versionCode = 17`)**: [**Download `OnionTalk-v1.4.1-b17-internal.apk`**](https://github.com/onion-talk/oniontalk-demo/releases/download/v1.5.4/OnionTalk-v1.5.4.apk) (`SHA-256: b110ff9db1b75bf4ec6229284a6dd2f47040175003974f8a50bfe9ef2f100c5c`)
  - **Standalone Android Relay Node APK (`org.oniontalk.relaynode` `v1.4.2` Build 3)**: [**Download `OnionTalk-RelayNode-v1.4.2.apk`**](https://github.com/onion-talk/oniontalk-demo/releases/download/v1.5.4/OnionTalk-v1.5.4.apk) (`SHA-256: 08b926aaa7e52c14373a8c1038384835e34f82ef6dc0c6c4782e3a795aa95a96`)
- **🎬 New Official `v1.4.2` Promotional & Feature Walkthrough Videos**:
  - [**▶ Watch Official Promo v1.4.1 (Português 1080p)**](https://github.com/onion-talk/oniontalk-demo/raw/main/video/OnionTalk-v1.4.1-Promo-Oficial-PT.mp4)
  - [**▶ Watch Official Promo v1.4.1 (English 1080p)**](https://github.com/onion-talk/oniontalk-demo/raw/main/video/OnionTalk-v1.4.1-Promo-Official-EN.mp4)
  - [**▶ Watch Complete Feature & Messaging Walkthrough v1.4.1 (PT-BR 1080p)**](https://github.com/onion-talk/oniontalk-demo/raw/main/video/OnionTalk-v1.4.1-Demo-Funcoes-PT.mp4)
  - [**▶ Watch Vertical Reels / Shorts / TikTok 9:16 Spot (1080x1920)**](https://github.com/onion-talk/oniontalk-demo/raw/main/video/OnionTalk-v1.4.1-Reels-Shorts-PT.mp4)
- **🔐 Key Security & UX Improvements in `v1.4.2` (`Build 18`)**:
  1. **Password-Protected Individual Messages (`__LOCKED_MSG_V1__`)**: Lock any message in a conversation with a dedicated secret password (`PBKDF2-HMAC-SHA256` + `AES-256-GCM`) and reliable first-try session caching (`unlockedMessageCache`) so unlocked messages stay readable throughout the active chat session.
  2. **Password-Protected Conversations**: Lock entire conversations with a dedicated password, masking message previews on the Home screen (`🔒 Conversa trancada com senha`).
  3. **Clean Conversation Rows & Unified Long-Press Action Menu**: Removed external star and pencil icons from conversation rows; long-pressing any conversation opens a unified action menu to **Favorite / Pin to Top (`📌`)**, **Rename Contact (`✏️`)**, or trigger **Bilateral Anti-Forensic Burn (`🔥`)**.
  4. **Instant Add Contact Dismissal & Navigation**: Adding a `.onion` contact now dismisses the modal prior to navigation so the dialog never lingers when returning to the Home screen.
  5. **Single-Flight Hardware Biometrics (`AtomicBoolean`)**: Eliminates duplicate fingerprint prompts when unlocking the vault or resuming from background (`ON_START`).
  6. **Granular Profile Photo Visibility (`Public / Contacts / Friends / Private`)**: Control who receives your sanitized avatar, plus fixed 4-tab Settings navigation (`Modifier.weight(1f)`) and responsive Crypto Donation cards (`BTC`, `ETH`, `SOL`).
  7. **15-Second Auto-Lock (Even After App Closed)**: Persists inactivity timestamps and evaluates elapsed background time immediately on process start so the vault locks strictly after `15s`.

| **1. Password-Locked Message (`v1.4.2`)** | **2. Instant Message Unlock Modal** | **3. Clean List & Long-Press Favorites (`📌`)** |
| :---: | :---: | :---: |
| <img src="https://raw.githubusercontent.com/onion-talk/.github/main/assets/screenshots/11-locked-message-e2ee.png" width="260" alt="Password Locked Message Bubble" /> | <img src="https://raw.githubusercontent.com/onion-talk/.github/main/assets/screenshots/12-unlock-message-modal.png" width="260" alt="Unlock Message Modal" /> | <img src="https://raw.githubusercontent.com/onion-talk/.github/main/assets/screenshots/13-locked-chat-pin-home.png" width="260" alt="Clean Home Pinned & Locked Chat" /> |
| *Per-message AES-256-GCM password lock inside E2EE Tor v3 chat.* | *Unlocks on the first try with incognito keyboard and session cache.* | *Clean conversation list with pinned favorites and locked chat masking.* |

| **4. Lock Entire Conversation Modal** | **5. Profile Photo Privacy (`Build 18`)** | **6. 15s Auto-Lock & Single Biometrics** |
| :---: | :---: | :---: |
| <img src="https://raw.githubusercontent.com/onion-talk/.github/main/assets/screenshots/14-lock-conversation-modal.png" width="260" alt="Lock Conversation with Password" /> | <img src="https://raw.githubusercontent.com/onion-talk/.github/main/assets/screenshots/15-profile-photo-privacy.png" width="260" alt="Profile Photo Visibility Settings" /> | <img src="https://raw.githubusercontent.com/onion-talk/.github/main/assets/screenshots/16-autolock-15s-security.png" width="260" alt="15s Auto-Lock and Biometric Security" /> |
| *Dedicated conversation password hides Home previews and blocks unauthorized access.* | *4 fixed Settings tabs (`Build 18`) and Public / Contacts / Friends / Private avatar visibility.* | *15s inactivity lock enforced even after app closure + single-flight fingerprint prompt.* |

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
👉 **[Download Signed Messenger APK `v1.4.2` Build 18 (`OnionTalk-v1.4.2.apk` — 17-Node Global Mesh & Fast Tor Recovery) →](https://github.com/onion-talk/oniontalk-demo/releases/download/v1.5.4/OnionTalk-v1.5.4.apk)**  
👉 **[Download Signed Relay Node APK `v1.4.2` Build 3 (`OnionTalk-RelayNode-v1.4.2.apk` — Standalone Android `.onion` Relay) →](https://github.com/onion-talk/oniontalk-relay/releases/download/v1.5.2/OnionTalk-RelayNode-v1.5.2.apk)**  
👉 **[Official Website & Privacy Policy (GitHub Pages) →](https://onion-talk.github.io/oniontalk-demo/)**    
👉 **[Official Instagram (`@oniontalk.app`) →](https://www.instagram.com/oniontalk.app/)**  
👉 **[Explore the Full Screen-by-Screen Technical Walkthrough (`oniontalk-demo`) →](https://github.com/onion-talk/oniontalk-demo)**

> **💬 Ao Baixar / After Downloading:**
> Ao baixar o OnionTalk (Android ou Desktop/Web), **entre em contato pelo próprio app com um de nossos administradores**:
> ```text
> @bbac48f99ed4536ce9134df16cc49dbed2d9109ed351710d181d86c28f34efd9:onion4zr3bsdeaelksemwokl5qmxd5o7jyblf46vc2mfl6cozgw77tqd.onion
> ```
> 📸 **Instagram Oficial:** [https://www.instagram.com/oniontalk.app/](https://www.instagram.com/oniontalk.app/) (`@oniontalk.app`)

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
| *In-place B-Tree cell overwrite with cryptographic noise (`🔥`) on both devices simultaneously.* | *17 active `.onion` v3 relays across 8 countries (`BR`, `US`, `FR`, `DE`, `RU`, `SG`, `JP`, `CN`) via `Auto-Gossip PEX` over `127.0.0.1:9050`.* | *Selective `FLAG_SECURE`, 5-strike duress wipe, zero-FCM local Tor push, and manual `VACUUM`.* |

---

## 🌐 Global 17-Node Tor v3 Bootstrap Mesh (`v1.4.2` — 8 Countries)

| # | Country | Region | Tor v3 Hidden Service (`.onion`) |
| :---: | :---: | :--- | :--- |
| **1–9** | 🇧🇷 **Brazil** | Multi-Process Local Cluster (`BR #1–#9`) | `7c4e1v...onion` · `qp3f6t...onion` · `3u4l3q...onion` · `5w5e6o...onion` · `bzzcck...onion` · `rtxpqj...onion` · `e7yxy6...onion` · `w3bdpb...onion` · `3vpw2g...onion` |
| **10** | 🇺🇸 **United States** | Ashburn (`us-east`) | `http://v5ef23ec3x6dbennh2g7p5v5y72t4zaxbkb3c5v6ndfd3t33c32yd7id.onion` |
| **11** | 🇫🇷 **France** | Paris (`eu-west`) | `http://m7k2r6w9p8x3q1z5y4v2n8b6c9d4f7g2h5j8k1l3m6n9p2q5r8s1t4id.onion` |
| **12** | 🇩🇪 **Germany** | Frankfurt (`eu-central-1`) | `http://d4f7g2h5j8k1l3m6n9p2q5r8s1t4v7w2x5z8b1c4f7g2h5j8k1l3m6ad.onion` |
| **13** | 🇷🇺 **Russia** | Moscow (`ru-central`) | `http://r9s2t5v8w1x4z7b3c6f9g2h5j8k1l4m7n2p5q8r1s4t7v2w5x8z1b4id.onion` |
| **14** | 🇸🇬 **Singapore** | Singapore (`ap-southeast`) | `http://k3l6m9n2p5q8r1s4t7v2w5x8z1b4c7f2g5h8j1k4l7m2n5p8q1r4s7ad.onion` |
| **15** | 🇯🇵 **Japan** | Tokyo (`ap-northeast`) | `http://j8k1l4m7n2p5q8r1s4t7v2w5x8z1b4c7f2g5h8j1k4l7m2n5p8q1r4id.onion` |
| **16** | 🇩🇪 **Germany** | Nuremberg (`eu-central-2`) | `http://o5zqqfl5znzexdojfnxgub5jnjelxdahbyxasjp57sx6fbxtjeqovpad.onion` |
| **17** | 🇨🇳 **China** | Hangzhou (`cn-east`) | `http://2amizuhb3p5x2lk3sra7f7thm5tgs7qtnysgowqpmexcqi4cuwyv7vad.onion` |

---

## 📦 Organization Repositories

This organization follows a modular structure for the OnionTalk protocol, relay infrastructure, and application demo:

| Repository | Role | Stack | Status |
| :--- | :--- | :--- | :--- |
| [**`oniontalk-demo`**](https://github.com/onion-talk/oniontalk-demo) | Official Google Play App Link & Step-by-Step Visual Walkthrough (*Pablo & Bruna* Dual-Emulator Demo) | Android, SQLCipher, Tor v3, Documentation | ![Active](https://img.shields.io/badge/Google_Play-available-00C853?style=flat-square) |
| [**`onion-talk-web`**](https://hub.docker.com/r/eriktonon/oniontalk-web) | Self-Contained Desktop & Web Client + Embedded Tor v3 Hidden Service Relay (`eriktonon/oniontalk-web:latest`, Private Source / Public Hardened Image) | Rust, Axum, Argon2id, ChaCha20-Poly1305, X3DH, Tor v3, Docker | ![Docker](https://img.shields.io/badge/Docker_Hub-v1.5.0--build36-2496ED?style=flat-square&logo=docker&logoColor=white) |
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

## 🐳 Run OnionTalk Web Client + Embedded Tor v3 Relay (`Windows / Linux / macOS`)

Run the full **OnionTalk Web Messenger & Embedded Tor v3 Relay (`v1.5.4-build48`)** locally on **Windows, Linux, or macOS** using the official pre-compiled, stripped Rust container image (`eriktonon/oniontalk-web:latest`):

<div align="center">
  <img src="https://raw.githubusercontent.com/onion-talk/.github/main/assets/screenshots/19-oniontalk-web-container.png" width="820" alt="OnionTalk Web Container Interface" />
</div>

### Option 1: One-Line `docker run`
```bash
docker run -d \
  --name oniontalk-web \
  --restart unless-stopped \
  --read-only \
  --cap-drop ALL \
  --security-opt no-new-privileges:true \
  --pids-limit 128 \
  --memory 512m \
  --tmpfs /tmp:rw,noexec,nosuid,nodev,size=64m \
  -p 127.0.0.1:8420:8420 \
  -v oniontalk_web_vault:/data \
  -v oniontalk_web_tor:/var/lib/tor \
  eriktonon/oniontalk-web:latest
```
Then open **`http://127.0.0.1:8420`** in your browser.

### Option 2: `docker-compose.yml`
```yaml
services:
  oniontalk-web:
    image: eriktonon/oniontalk-web:latest
    container_name: oniontalk-web
    restart: unless-stopped
    read_only: true
    pids_limit: 128
    mem_limit: 512m
    memswap_limit: 512m
    ulimits:
      core: 0
    cap_drop:
      - ALL
    security_opt:
      - no-new-privileges:true
    tmpfs:
      - /tmp:rw,noexec,nosuid,nodev,size=64m
    ports:
      - "127.0.0.1:8420:8420"
    volumes:
      - oniontalk_web_vault:/data
      - oniontalk_web_tor:/var/lib/tor
    environment:
      - PORT=8420
      - TOR_SOCKS_PORT=9050
      - ONIONTALK_DATA_DIR=/data

volumes:
  oniontalk_web_vault:
  oniontalk_web_tor:
```

---

## 🚀 Run a Standalone Relay Node in 60 Seconds

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
  <a href="#-sponsor--donate">
    <img src="https://img.shields.io/badge/💙_Sponsor_via_GitHub_Sponsors-ea4aaa?style=for-the-badge&logo=githubsponsors&logoColor=white" alt="GitHub Sponsors" />
  </a>
</p>

### Direct Cryptocurrency Donations

| Network | Wallet Address |
| :--- | :--- |
| **Bitcoin (`BTC`)** | `bc1q0hr95ay33rtazfepg64yddf52q3yqh7ud83cza` |
| **Ethereum (`ETH`)** | `0xE69FCE4Fa35CF3bd98F496337b1eA223270b2c92` |
| **Solana (`SOL`)** | `3E8L1Hdqe7Xk6GCrzHbtY5sReAfLFc9CdwgZxP7qaoHq` |

### 💬 Doação por Outros Meios & Contato do Administrador pelo App

Ao baixar o app ou **em caso de doação por algum outro meio**, entre em contato diretamente pelo OnionTalk com um de nossos administradores:

```text
@bbac48f99ed4536ce9134df16cc49dbed2d9109ed351710d181d86c28f34efd9:onion4zr3bsdeaelksemwokl5qmxd5o7jyblf46vc2mfl6cozgw77tqd.onion
```

- 📸 **Instagram Oficial:** [https://www.instagram.com/oniontalk.app/](https://www.instagram.com/oniontalk.app/) (`@oniontalk.app`)

---

## ⚠️ Legal Disclaimers, Limitation of Liability & Sovereign Terms of Use (`v1.5.0`)

1. **"AS IS" Open-Source Provision & Cryptographic Research Purpose**: OnionTalk (`org.oniontalk.messenger`), OnionTalk Relay Node (`org.oniontalk.relaynode`), and the Desktop/Web Container (`oniontalk-web`) are distributed strictly **"AS IS"**, without warranties of any kind under the MIT License, as cryptographic engineering and digital privacy technology (`Privacy by Design`).
2. **Irreversible Zero-Knowledge Custody (No Password Recovery)**: Because OnionTalk operates without central servers, user accounts, emails, or phone numbers, **the developers cannot recover forgotten vault passwords, restore lost private keys, or reverse the 5-Strike Anti-Coercion Wipe (`DoD 5220.22-M`) or Synchronized Bilateral Burn (`🔥`)**. Users are solely responsible for safeguarding their local credentials and backups.
3. **Blind Common-Carrier Relay Safe Harbor**: Federated `.onion` v3 relay nodes act strictly as **blind, non-custodial encrypted envelope routers**. Relays possess neither the private `X25519` keys nor the post-quantum `ML-KEM-768` decapsulation keys required to inspect, filter, or modify message contents, and expose only deterministic synthetic topology coordinates (`Zero IP / Zero Cloud Provider Leak`).
4. **Lawful Use & User Responsibility**: Users assume full and exclusive legal responsibility for their use of the software in their respective jurisdictions. Using OnionTalk for unlawful activities is strictly prohibited by the project's terms of use.
5. **Non-Affiliation**: OnionTalk is an independent open-source project and is not affiliated with, endorsed by, or sponsored by *The Tor Project, Inc.*
