# PABRIK ROTI [![version](https://img.shields.io/badge/version-2.3.33-blue)](https://github.com/myreceiptt/pabrikroti-master/releases/tag/v.2.3.33-far)

> "This is not just a factory. This is a rehearsal of freedom—kneaded with code, fermented by its community, and baked through the heat of shared struggles."
>
> — Prof. NOTA

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

---

---

## PABRIK ROTI v.2.3.33: Staging NFT FAR by Futuloka

Link #1: [far.futuloka.io](https://far.futuloka.io/)  
Link #2: [www.futuloka.xyz](https://www.futuloka.xyz/)  
Link #3: [far.futuloka.xyz](https://far.futuloka.xyz/)  
Link #4: [far.endhonesa.com](https://far.endhonesa.com/)

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

## Evergreen Notes

- `@types/node` is pinned to **24.x** to match the Node 24 runtime (Vercel).
- Yarn is **4.x**; use `yarn outdated` for update review and `yarn npm audit --severity moderate` for security checks.

## Join Prof. NOTA Discord

For questions or suggestions, join Prof. NOTA discord at [https://discord.gg/5KrsT6MbFm](https://discord.gg/5KrsT6MbFm).
