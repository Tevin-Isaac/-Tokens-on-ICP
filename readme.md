# Table of Contents

- [🪙 Tokens on ICP](#-tokens-on-icp)
  - [💼 Token Use Cases & Utility Examples](#-token-use-cases--utility-examples)
- [🟡 Token Standards](#-token-standards)
- [💠 ICRC-1 Token Standard](#-icrc-1-token-standard)
  - [🔍 Example ICRC-1 Tokens](#-example-icrc-1-tokens)
  - [💻 Code Examples for ICRC-1 Transfers](#-code-examples-for-icrc-1-transfers)
- [🚀 Recommended Token Launch Platforms](#-recommended-token-launch-platforms)
  - [🔥 Meme Token Launchers](#-meme-token-launchers)
  - [₿ Bitcoin-style Tokens / NFT Ordinals](#-bitcoin-style-tokens--nft-ordinals)
  - [🏛 DAO Launchers](#-dao-launchers)
  - [💼 Token Launchpads / Fundraising](#-token-launchpads--fundraising)
  - [🤖 Utility / AI Tokens](#-utility--ai-tokens)
  - [🛠 Under Active Development](#-under-active-development)
- [🔄 Token Swapping & Liquidity](#-token-swapping--liquidity)
- [📊 Token Metrics & Analytics](#-token-metrics--analytics)
- [✍️ Want to Create Your Own Token?](#️-want-to-create-your-own-token)
  - [🧑‍🎓 Bonus Learning Resources](#-bonus-learning-resources)
- [✅ Final Notes](#-final-notes)

## 🪙 Tokens on ICP
![Image](https://github.com/user-attachments/assets/ecfb80ef-3c86-461e-b9d1-47a170f8a72c)

The DeFi ecosystem on the Internet Computer (ICP) includes three main asset types:

* **ICP token**: The network's native utility token.
* **Cycles**: The equivalent of "gas" on ICP.
* **ICRC tokens**: Tokens that follow ICRC standards (fungible + non-fungible).

---

### 💼 Token Use Cases & Utility Examples
* **Governance** (e.g. SNS DAO voting power)
* **Rewards** (community, staking, quests)
* **Payments** (buying digital goods/services)
* **Access** (gated content, AI tools, NFT mints)
* **Meme/Community** tokens that go viral


## 🟡 Token Standards

The Internet Computer uses **ICRC (Internet Computer Request for Comments)** token standards.

| Standard | Type         | Description                                     | Similar To       |
| -------- | ------------ | ----------------------------------------------- | ---------------- |
| ICRC-1   | Fungible     | Base fungible token (transfer, balanceOf)       | ERC-20           |
| ICRC-2   | Fungible     | Adds delegated transfers (approve/transferFrom) | ERC-20 + approve |
| ICRC-7   | Non-Fungible | NFT standard on ICP                             | ERC-721          |
| ICRC-37  | Non-Fungible | Extends ICRC-7 with approval workflows          | ERC-1155 vibes   |

> Most token launch platforms use **ICRC-1** as the default for fungible tokens.

---

## 💠 ICRC-1 Token Standard

**ICRC-1** is the base standard for fungible tokens on ICP. It intentionally excludes certain features, such as:

* Smart contract transaction notifications
* Pre-signed transactions
* Block structures or fetchable transaction blocks

ICRC-1 is designed to be lightweight and extendable. The `icrc1_supported_standards` endpoint can be queried to find additional extensions supported by a token.

### 🔍 Example ICRC-1 Tokens:

| Token                                                               | Description                      | Link    |
| ------------------------------------------------------------------- | -------------------------------- | ------- |
| [ICX](https://icpex.org/token/detail/lvfsa-2aaaa-aaaaq-aaeyq-cai)   | A standard ICRC-1 fungible token | ICPex |
| [HOT](https://icpex.org/token/detail/rrkah-fqaaa-aaaaa-aaaaq-cai)   | ICRC-1 token                     | ICPex |
| [PANDA](https://icpex.org/token/detail/bv6fl-sqaaa-aaaaq-aae3a-cai) | ICRC-1 token                     | ICPex |
        
---

### 💻 Code Examples for ICRC-1 Transfers

#### ✅ Motoko Example (Transfer)

```motoko
let transferArgs = {
  from_subaccount = null;
  to = recipientPrincipal;
  amount = 1000000;
  fee = null;
  memo = null;
  created_at_time = null;
};
let result = await tokenActor.icrc1_transfer(transferArgs);
```

#### ✅ Rust Example (Transfer)

```rust
let args = TransferArg {
    from_subaccount: None,
    to: recipient_principal,
    amount: 1_000_000,
    fee: None,
    memo: None,
    created_at_time: None,
};
let result = token_canister.icrc1_transfer(args).await?;
```

🔗 View [ICRC-1 Methods Documentation](https://github.com/dfinity/ICRC-1/tree/main/standards/ICRC-1)

---

## 🚀 Recommended Token Launch Platforms

A curated list of **actively maintained token launchers** on ICP—great for developers, meme lords, and builders.

### 🔥 Meme Token Launchers

1. **[launch.bob.fun](https://launch.bob.fun/)**

    * Dead simple meme-token launcher
    * Community-focused

2. **[icpex.org/createToken](https://icpex.org/createToken)**

    * Launch & swap tokens
    * Good traction for early tokens

3. **[Fomowell](https://fomowell.com/board)**

    * Low-cost meme coins
    * AI + content on-chain

4. **[Pacapump](https://pacapump.io/)**

    * Launch, manage, and trade IC tokens

---
### ₿ Bitcoin-style Tokens / NFT Ordinals
* **[Odin Fun](https://odin.fun/)**

  * Hybrid between meme tokens & NFT inscriptions

---

### 🏛 DAO Launchers

* **[nns.ic0.app/launchpad](https://nns.ic0.app/launchpad)**

  * Launch SNS DAOs with built-in governance

---

### 💼 Token Launchpads / Fundraising

* **[Launchpad on ICTO](https://icto.app/launchpad)**

  * Streamline vesting, payroll, and token launches

* **[icptokens.com](https://icptokens.com/)**

  * Directory of available launchpads on ICP

---

### 🤖 Utility / AI Tokens

* **[Elna](https://www.elna.ai/)**

  * First on-chain AI companion dapp

---

### 🛠 Under Active Development

* **[IC Toolkit](https://ic-toolkit.app/browse)**

  * Multi-tool for NFTs, dapps, and token deployment




### 🔄 Token Swapping & Liquidity


* How ICRC-1 tokens are traded/swapped on:

  * [ICPSwap](https://icpswap.com/)
  * [Sonic](https://sonic.ooo/)
  * [ICPex](https://icpex.org/)
![Image](https://github.com/user-attachments/assets/9223f073-afd8-4c9f-991b-1d319fc09541)



### 📊 Token Metrics & Analytics

* Platforms:

  * [DexScreener for IC](https://dexscreener.com/icp)

  * [ICP Swap](https://info.icpswap.com/)

## ✍️ Want to Create Your Own Token?

You can directly create and deploy **ICRC-1 tokens** using:

* `dfx` CLI with Motoko or Rust
* SDKs like `ic-js`, `ickit`, or `Azle` (TypeScript)
* The ledger canister

### 🧑‍🎓 Bonus Learning Resources
Learn more how to build on ICP here
* [awesome-education-hub](https://github.com/ICP-HUBS-DevRels-Syndicate/awesome-education-hub.git)


## ✅ Final Notes
When launching a token:
* Focus on **traction** + **community support**
* Avoid abandoned or unmaintained platforms
* Choose the right standard (ICRC-1 or ICRC-7) based on your use case