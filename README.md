# 🚨 Project R3APΞX: Real Racing 3 Server Emulator

> **SYSTEM STATUS:** UPLINK ACTIVE // AWAITING CLIENT CONNECTION
> **TARGET SHUTDOWN DATE:** March 20, 2026

## 📖 About The Project

As announced, the official EA servers for Real Racing 3 are scheduled for a permanent blackout on **March 20, 2026**. For most players, this means the end of the road. 

**Project R3APΞX** is a custom, independent Server Emulator developed to keep players racing career alive indefinitely. By intercepting and rerouting the game's network traffic through DNS/Proxy hijacking, R3APΞX safely bypasses the dead official servers and restores core online functionality. 

This solution is **100% platform-agnostic**. It works natively on both **iOS and Android** using the untouched, official game client—no root, no jailbreak, and no modded binaries required.

---

## ⚙️ Features Restored

When your device handshakes with the R3APΞX network, you retain access to these vital features:
* 🎁 **Daily Login System:** Your login streaks remain intact. Daily rewards are distributed normally by the private node.
* 💰 **Economy Injection:** M&#36; endpoints are fully rerouted. You can continue acquiring M&#36;.
* ⏱️ **Chrono Syncing:** Server timestamps are accurately simulated. All **Servicing & Upgrade** countdown timers sync seamlessly (no infinite waiting glitches).
* 🏁 **Special Events Portal:** The time-limited event gateway has been forced open, making Special Events accessible via the private uplink.

---

## 🔀 Dual Server Nodes: Choose Your Timeline

The R3APΞX infrastructure features two distinct routing endpoints. You can configure your routing utility to point to the node that fits your playstyle:

### 🟢 Node 1: The Legacy Timeline (Vanilla Experience)
* **Endpoint URL:** `$project-r3apex-server$/legacy`
* **Mechanics:** The server heartbeat synchronizes strictly with the real-world clock (1:1 time scale). 
* **Details:** Once connected to this node, any expired Round Hub events will remain permanently locked. Your gameplay will perfectly mirror the exact "end-of-life" maintenance state of the game during its final 3 months.

### 🟣 Node 2: The Accelerated Round Hub (Time-Warp)
* **Endpoint URL:** `$project-r3apex-server$/roundhub`
* **Mechanics:** Designed specifically for players who missed past roundhub events and want a second chance. The server timestamp operates on a continuous loop from **August 2021 (Season 1, Round 1)** to **December 2025 (Season 5, Round 3)**.
* **Time Dilation:** The clock on this node runs at **6x real-world speed** (i.e., 4 real-world hours = 1 in-game day). For example, a typical Round that originally lasted 6 weeks (42 in-game days) will cycle through in just **7 real-world days** (42 ÷ 6).
* **The Trade-off (Daily Streaks):** While this acceleration drastically eliminates agonizing seasonal wait times, it severely compresses the daily login reward cycle. Since an in-game "day" resets every 4 real-world hours, you must boot the game much more frequently to maintain a perfect login streak.

---

## 🌍 How to Connect

### Method A: Official Client via Network Routing (iOS & Android)
If you want to use the untouched official game from the App Store or Google Play, you must utilize network-level redirection. 

> **🛡️ Security & Privacy Notice:** > Players who prefer the official client over patched binaries typically do so out of strict security and privacy principles. Respecting that mindset, **I will not provide detailed tutorials on network traffic hijacking, nor will I recommend or endorse any specific proxy/DNS applications.** This ensures complete project neutrality. You are responsible for independently researching how to execute URL rewriting and MITM (Man-in-the-Middle) redirection using your preferred tools, search engines, or AI assistants.

1. **Acquire a Routing Utility:** Procure a network proxy or routing application for your device that is capable of URL Rewriting and MITM decryption.
2. **Obtain the Ruleset:** Open the `R3APEX_Routing.conf` file located in the root directory of this repository. You can download the file directly or copy its raw text contents.
3. **Configure the Node:** Edit the configuration and ensure the target points to your preferred Node (`/legacy` or `/roundhub`).
4. **Engage the Uplink:** Import the ruleset into your routing app and toggle the VPN profile **ON**.
5. **Launch RR3:** Open your game. The traffic will automatically bypass the dead EA domains and handshake with the R3APΞX server.

### Method B: The Modded APK (Android Only)
If you prefer a plug-and-play experience without manually configuring network routing or proxy tools, you may search the internet or modding forums for pre-configured Mod APKs created and hosted by independent third-party communities.

*Note: To strictly comply with copyright policies, this repository does NOT provide, host, or link to any modified client executables or game assets.*

---

## ⚠️ Critical Infrastructure Constraints

Project R3APΞX is currently deployed entirely on free-tier serverless and hosting networks. Consequently, the node faces strict hardware quotas regarding bandwidth, daily request limits, and database storage capacity. 

To ensure the core systems remain stable and free for everyone, the following high-concurrency and high-bandwidth modules have been **suspended**:

1. 🚫 **No Asset Downloads:** R3APΞX does **NOT** host the massive in-game `.depot` asset files. You **MUST** let the game download all required tracks, cars, and assets via the official EA servers **BEFORE** the blackout date. Once EA shuts down, missing game files cannot be retrieved through R3APΞX.
2. 🚫 **No Cloud Saves:** The Cloud Sync module is explicitly disabled to conserve server load and database space. **R3APΞX will not back up your progress.** You are 100% responsible for your own data. Please manually back up your `character.dat` file locally.
3. 📊 **No Time Trial:** Maintaining global leaderboards demands rapid, high-volume database I/O, which immediately exceeds free-tier database quotas.
4. 🛡️ **No Race Teams:** Real-time team chat and member synchronization require sustained server capacity and concurrent connections that the current infrastructure cannot support.

---

## 📜 Disclaimer / Legal Notice
*Project R3APΞX is an independent, non-profit educational and reverse-engineering project dedicated strictly to software preservation. It is not affiliated with, endorsed by, or sponsored by Electronic Arts (EA), Firemonkeys Studios, or Slingshot. All trademarks, service marks, and copyrights are the property of their respective owners.*

**No Distribution of Copyrighted Material:** This repository is an original server emulation codebase. It does NOT contain, distribute, or host any copyrighted game assets, client executables (APKs/IPAs), or intellectual property belonging to EA. 

**User Responsibility and Assumption of Risk:** By redirecting your game client to connect to the R3APΞX network, you explicitly acknowledge that modifying your client or network traffic may violate the original Terms of Service (TOS) or End User License Agreement (EULA) of Real Racing 3.  End users are solely responsible for ensuring their actions comply with applicable laws and their own user agreements.
