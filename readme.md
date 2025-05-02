
## Tokens
On ICP, the DeFi ecosystem includes three types of assets:

- ICP token: The network’s native utility token.

- Cycles: The equivalent of “gas” on ICP.

- ICRC tokens: Tokens that adhere to a set of ICRC standards used for defining fungible and non-fungible tokens.

### 🟡 Token Standards

The Internet Computer supports token standards under the **ICRC (Internet Computer Request for Comments)** initiative.

- **ICRC-1**: Fungible token base standard (similar to ERC-20)
- **ICRC-2**: Adds approvals for delegated transfers
- **ICRC-7**: NFT standard for non-fungible tokens
- **ICRC-37**: The ICRC-37 standard is an extension of ICRC-7 that provides additional functionality for an approval workflow.

> Most token launch platforms currently adopt **ICRC-1** as the base fungible token standard.


## ICRC1
ICRC-1
The ICRC-1 standard is for fungible tokens on ICP. It is considered the 'base' standard and intentionally excludes certain features and functions, such as:

* Reliable transaction notifications for smart contracts.

* A block structure and the interface for fetching blocks.

* Pre-signed transactions.

ICRC-1 supports extensions of this standard to implement these missing functions, and the icrc1_supported_standards endpoint can be queried to return the name of all supported extensions.

Example ICRC-1 tokens on ICP include:

 **[ICX](https://icpex.org/token/detail/lvfsa-2aaaa-aaaaq-aaeyq-cai)**  


View an example dapp for ICRC-1 transfers.(https://github.com/dfinity/ICRC-1/tree/main/standards/ICRC-1)
Check the full ICRC1 token standard here(https://github.com/dfinity/examples/tree/master/motoko/token_transfer)

Learn more here (https://internetcomputer.org/docs/defi/token-standards/)


## 🧠 ICP Token Launch Platforms

Welcome to this curated list of **active and relevant token launch platforms** on the Internet Computer (ICP), specifically designed to help developers, meme lords, DeFi explorers, and Web3 founders launch tokens with clarity and purpose.

This list focuses on what's working *now*, prioritizing tools and platforms with real usage, volume, or traction. Dead projects, broken launchers, and non-maintained repos have been excluded intentionally.



### 🚀 Recommended Token Launch Platforms


#### 🔥 If you're launching an **IC-only Meme Token**:
Best platforms to go viral and get launched quickly:

1. **[bob.fun](https://bob.fun/)**  
   - Easiest meme-token launcher
   - User-friendly interface
   - Focused on the community/token virality
  
2. **[ICPex](https://icpex.org/)**  
   - Good meme-token traction
   - Offers launching and swapping
   - Early-stage token marketplace included


3. **[Fomowell](https://fomowell.com/board)**  
   - Issue low-cost meme coins with AI intergration and on-chain content management via ICP.

4. **[Pacapump](https://pacapump.io/)**  
   - Launch manage and trade tokens on IC.

---

#### ⚡ If you're building a **Bitcoin-style Meme Token** (IC-powered):
Use this if you want to experiment with NFT Ordinals or hybrid tokens:

- **[Odin Fun](https://odin.fun/)**  
  - Runes + IC-powered innovation  
  - Meme-token vibes with NFT-style data inscription

---

#### ⚡ If you're building a **DAO** (IC-powered):
This dapp allows you to manage ICP, stake neurons, participate in voting, and earn governance rewards.:

- **[NNS](https://nns.ic0.app/)**  
  - Launch SNS DAOs to transform dapps into community-owned ecosystems with built in governance tokens

---


#### ⚡ If you're building an **ICTO launchpad** (IC-powered):
This 

- **[Launchpad](https://icto.app/launchpad)**  
  - Streamline token vesting,payroll and fundraising on the Internet Computer Blockchain.

---

#### 👾 If you're launching an **IC Agent Token** (DeFi, Utility, Governance):

- **[Elna](https://www.elna.ai/)**  
  - ELNA.ai is the world's first fully onchain decentralized GenAI Companion.
 

---

### 🛠️ Under Active Development (Worth Watching)

- **[IC Toolkit](https://ic-toolkit.app/browse)**  
  - Incubated by PT/FR Hub  
  - Meant for broader use cases (NFTs, dapps, tokens)

---

### ✍️ Want to Create Your Own Token?

You can also directly create and deploy **ICRC-1 tokens** using tools like:
- `dfx` with Motoko/Rust boilerplates
- SDKs like `ic-js`, `ickit`, or `Azle` (TypeScript)
- Using Ledger canister.Learn how to do that here(https://github.com/ICP-Hub-Kenya/icp-token-creation)

---

### 💡 Final Notes

- Stay away from launchpads without volume or support
- Focus on community traction + technical reliability


---

