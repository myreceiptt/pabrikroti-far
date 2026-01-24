# PABRIK ROTI [![version](https://img.shields.io/badge/version-2.3.33-blue)](https://github.com/myreceiptt/pabrikroti-master/releases/tag/v.2.3.33-far)

> "This is not just a factory. This is a rehearsal of freedom—kneaded with code, fermented by its community, and baked through the heat of shared struggles."
>
> — Prof. NOTA

## PABRIK ROTI v.2.3.33: Staging NFT FAR by Futuloka

Link #1: [far.futuloka.io](https://far.futuloka.io/)  
Link #2: [www.futuloka.xyz](https://www.futuloka.xyz/)  
Link #3: [far.futuloka.xyz](https://far.futuloka.xyz/)  
Link #4: [far.endhonesa.com](https://far.endhonesa.com/)

## About This Repo

This repo powers **NFT FOR A REASON (NFT FAR)** — a Web3 initiative for grassroots culture & creative solidarity in Indonesia. The app publishes the program narrative (open call, curation, roadmap), then provides a gated onchain interface to collect curated NFTs and access supporting utilities and documents.

### What this app does

- **Landing + program pages** that explain the mission, participants, fund distribution, and the first supported project (**Festival Mbok Sri 2025**).
- **NFT collection flows** for free and paid editions (`/free`, `/paid`, `/token/[idNFT]`) with onchain supply, pricing, eligibility, and wallet-balance checks.
- **FT utilities** (`/coins`, `/address/[coinAddress]`) that expose claim/buy mechanics for fungible tokens used by the program (e.g., participation and future utility layers).
- **Search + featured discovery** (`/search`, `/featured`) to help users navigate content and drops.
- **Terms page** (`/terms`) driven by the active receipt configuration.

### Blockchain & smart accounts

- Multichain design with production deployment on **Base** and **Optimism (OP Mainnet)**.
- Wallet onboarding uses **thirdweb account abstraction** to provision **Smart Accounts** (with gas sponsorship enabled), plus supports in-app wallets (email/passkey/social) and external wallets.

### Technology

- Next.js (App Router) + React + TypeScript
- Tailwind CSS
- thirdweb SDK v5 (ERC-1155 / ERC-20 integrations + Smart Accounts)
- Vercel deployment

### How we build (quality + workflow)

- We keep the UI production-safe and the onchain logic auditable: each claim path reflects live chain state (eligibility, supply, max supply, and currency).
- We ship changes in small, reviewable steps with consistent maintenance (Node / Yarn), and always verify with audit/lint/build.
- We treat this repo as an operational artefact: a documented program interface that stays deployable while preserving the intent and UX of the initiative.

## 📜 Licenses

This project is licensed under a [**Custom Limited License**](./LICENSE) by [Prof. NOTA & Prof. NOTA Inc.](https://nota.endhonesa.com/).

- 🏛️ [English (UK)](./licenses/LICENSE_en-GB.md)
- 🇮🇩 [Bahasa Indonesia](./licenses/LICENSE_id.md)
- 🇺🇿 [Oʻzbekcha](./licenses/LICENSE_uz-Latn.md)
- 🇭🇰 [Cantonese – Hong Kong](./licenses/LICENSE_yue-Hant-HK.md)
- 🇲🇾 [Bahasa Malaysia](./licenses/LICENSE_ms-MY.md)
- 🇦🇪 [العربية – الإمارات](./licenses/LICENSE_ar-AE.md)

> 📩 For permission or inquiries, contact: [nota@endhonesa.com](mailto:nota@endhonesa.com)

## 📜 Manifestos

If you already have obtained the license, please read and understand the manifesto from [Prof. NOTA & Prof. NOTA Inc.](https://nota.endhonesa.com/) before starting to use it.

- 🏛️ [English (UK)](./manifestos/manifesto_en-GB.md)
- 🇮🇩 [Bahasa Indonesia](./manifestos/manifesto_id.md)
- 🇺🇿 [Oʻzbekcha](./manifestos/manifesto_uz-Latn.md)
- 🇭🇰 [Cantonese – Hong Kong](./manifestos/manifesto_yue-Hant-HK.md)
- 🇲🇾 [Bahasa Malaysia](./manifestos/manifesto_ms-MY.md)
- 🇦🇪 [العربية – الإمارات](./manifestos/manifesto_ar-AE.md)

## Usage

### Install dependencies

```bash
yarn install
```

### Review dependency updates (interactive)

```bash
yarn up -i
```

### Upgrade dependencies

```bash
yarn up -R
```

### Start development server

```bash
yarn dev
```

### Check all the code

```bash
yarn lint
```

### Create a production build

```bash
yarn build
```

### Preview the production build

```bash
yarn start
```

## Resources

- [Prof. NOTA Inc.](https://nota.endhonesa.com/)
- [Prof. NOTA Console](https://prompt.endhonesa.com/)
- [Prof. NOTA Tutor](https://baca.endhonesa.com/)

## Join Prof. NOTA Discord

For questions or suggestions, join Prof. NOTA discord at [https://discord.gg/5KrsT6MbFm](https://discord.gg/5KrsT6MbFm).

---

---

## Maintenance by Prof. NOTA Evergreen Standard

This repo is intended to stay evergreen while remaining production-safe.

### Current Baseline (Jan 2026)

- Runtime: Node **24.x** (Vercel-compatible; see `.nvmrc` and `package.json#engines`)
- Package manager: Yarn **4.12.0** (lockfile: `yarn.lock`)
- Types: `@types/node` **24.10.7** (pinned to match Node 24; 25.x intentionally deferred)
- Key packages: Next.js **16.1.4**, React **19.2.3**, thirdweb **5.118.0**, framer-motion **12.29.0**
- Deploy target: **Vercel auto-deploy from `main`**

### Monthly Evergreen Cycle (safe)

- `yarn install`
- `yarn up -R "*"`
- `yarn npm audit --severity moderate`
- `yarn lint`
- `yarn build`

### Quarterly Evergreen Cycle (major review)

- Review majors one at a time (framework/tooling), with a dedicated PR.
- If `@types/node` gets bumped, repin to **24.10.7**, then re-run audit/lint/build.
