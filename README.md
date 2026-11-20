# A7A5-Trace — Web3 Intelligence Dashboard on Crypto-Energy Sanctions Evasion

## What is A7A5-Trace?

A7A5-Trace is a free, interactive dashboard that dissects the **A7A5 token**: a ruble-backed stablecoin used to facilitate ruble-denominated energy payments while circumventing SWIFT and OFAC controls.

Think of it as a hands-on investigation file. Instead of reading scattered sanctions notices and analytics reports, you click through an animated crypto-energy transfer network, filter indicators of compromise, walk through investigation scenarios and explore the full entity circuit behind the token: **A7 LLC, the Kyrgyz issuer nodes, Promsvyazbank and the Hong Kong gateway**.

The dashboard was built as teaching material for the **second hands-on forensic investigation workshop funded by a Solana Foundation grant**.

## Why Was This Dashboard Built?

Future legal professionals (prosecutors, judges, compliance officers and regulators) graduate without any practical understanding of how blockchain ecosystems are weaponized for terrorism financing and international sanctions evasion.

This creates a critical enforcement gap. Courts and regulators are confronted with on-chain evidence they cannot evaluate. Meanwhile, bad actors operate with near-impunity in jurisdictions where legal expertise hasn't caught up with Web3 realities.

A7A5 is the clearest example of that gap today. Its reserves sit at a sanctioned Russian state bank, out of reach of Western freeze orders, and its volume runs through Kyrgyz shells, OTC desks and exchanges designed to avoid centralized KYC/AML. Investigators who only know how to trace SWIFT messages cannot follow it. Investigators who can read the ledger can.

It is imperative for us, experts in our field, to share our expertise in the best way possible, and hands-on workshops are the best way to impact the community. This dashboard is the material behind that workshop, released openly so anyone can teach with it.

## How Simple Is It?

This project is intentionally basic and straightforward:

- No frameworks like React or Vue.js. Just **one `index.html` file**: HTML, CSS and vanilla JavaScript
- Works in any modern web browser, on desktop and mobile
- No installation, no build step, no backend
- No API key required

Perfect for trainers, students, investigators and compliance teams who want to open it and start teaching or learning right away.

## What You Get

The dashboard is organized in two parts.

### Part I — Web3 Intelligence on the Crypto-Energy Transfer Network

| Section | What it shows |
|---|---|
| **Workshop** | What the workshop covers and who it's for |
| **Why It Matters** | Why on-chain intelligence beats traditional AML against A7A5, and why USDT freezes work while A7A5 freezes don't |
| **Flow Analysis** | Animated network map: sanctioned energy proceeds → PSB minting → exchanges → Dubai, Hong Kong and Istanbul off-ramps |
| **Methodology** | A 5-phase investigation protocol, from seeding OFAC SDN addresses to multi-jurisdiction seizure |
| **Case Studies** | Three interactive scenarios: OTC desk identification, DEX liquidity trace, fiat off-ramp takedown |
| **IOCs** | 9 indicators of compromise, filterable by severity (critical, high, medium) |
| **Tools** | The forensic toolkit by function: explorers (Tronscan, Etherscan), commercial analytics, OSINT and more |
| **Threat Evolution** | Forward-looking threat vectors: successor tokens, China integration, non-USD stablecoins, CBDC risk |

### Part II — The A7A5 Entity Circuit

| Section | What it shows |
|---|---|
| **Token** | How A7A5 works: ruble peg, staking yield, issuance chains and mechanics |
| **Ilan Shor** | Profile of the principal architect behind the scheme |
| **Entities** | Every actor in the circuit, with role, jurisdiction and sanctions status |
| **Entity Circuit** | Animated diagram linking political finance, state energy, issuance, exchange and exit layers |
| **Promsvyazbank** | Why the reserve bank is the "fortress" that makes A7A5 hard to freeze |
| **Timeline** | Key events from launch to sanctions designations |
| **Targeting** | Where investigators can realistically apply pressure on the circuit |

It also includes a **GDPR-compliant cookie banner and policy** (consent-first Google Analytics, optional preference cookies, full policy in a modal).

## Quick Setup (2 Minutes)

### Option 1: Just open it
1. Download `index.html` from this repository
2. Double-click it to open it in your browser

That's it. Everything works offline except the fonts and libraries loaded from CDNs.

### Option 2: Host it on your website
1. Upload `index.html` to any web hosting provider (or enable **GitHub Pages** on this repository)
2. Open your site's URL

### Optional: Enable Google Analytics
Analytics is **off by default**. To turn it on:

1. Open `index.html` in any text editor
2. Find the line: `window.CS_GA_ID = 'G-XXXXXXXXXX';`
3. Replace `G-XXXXXXXXXX` with your own GA4 Measurement ID
4. Save and upload

Google Analytics only loads **after** a visitor clicks *Accept* in the cookie banner.

### Optional: Adapt the cookie policy
The cookie policy names **Crypto Sentinel (gabidumitriu.ro)** as the data controller. If you host your own copy, edit the *"Who we are"* paragraph in the cookie modal so it names you instead.



## Technical Details

- **Stack:** HTML5, CSS3, vanilla JavaScript, Bootstrap 5.3.2
- **Libraries (via CDN):** Bootstrap and Bootstrap Icons (jsDelivr), Google Fonts (Rajdhani, DM Sans, Space Mono)
- **Cookies used:**
  - `cs_consent`: strictly necessary, stores your cookie choice (180 days)
  - `cs_prefs`: preferences, only with consent, remembers the open case-study scenario and IOC filter (180 days)
  - `_ga`, `_ga_<ID>`: Google Analytics, only with consent and only if a Measurement ID is configured
- **Fallback:** if the browser blocks cookies (for example, when opened as a local file), the choice is stored in `localStorage` instead

## Data Sources

- OFAC SDN List and Treasury press releases
- EU Council sanctions decisions
- Public research and reporting by TRM Labs, Chainalysis and Elliptic
- On-chain data (Tron and Ethereum)

## Limitations

- **Educational material, not legal advice.** Always verify against official OFAC, EU and UN publications before acting.
- Case studies are **realistic training scenarios** built on the A7A5 network typology. They are not open investigations.
- Figures (volumes, supply, seizures) reflect public reporting at the time the dashboard was prepared and will change. Check current sources before citing them.


## Troubleshooting

**Icons or fonts not showing?**
- You're probably offline. The libraries and fonts load from CDNs and need an internet connection.

**Cookie banner keeps appearing?**
- Your browser may be blocking both cookies and local storage (for example, strict private mode). The choice is then kept only for the current visit.

**Analytics not recording anything?**
- Check that you replaced `G-XXXXXXXXXX` with a real Measurement ID and that you clicked *Accept* in the cookie banner.

## Privacy & Security

- No backend, no database, no accounts
- No personal data is collected unless a visitor explicitly consents to Analytics
- No advertising, remarketing or social-media cookies
- Consent can be changed or withdrawn at any time from the cookie button in the bottom-left corner

## Disclaimer

This dashboard is independent analytical commentary based on public sources. It is not affiliated with or endorsed by OFAC, the EU, TRM Labs, Chainalysis, Elliptic or the Solana Foundation. References to individuals and entities reflect public sanctions designations and published reporting.

## Contributing

This is an open-source project funded by a grant powered by the Solana Foundation: https://earn.superteam.fun/grants/solana-foundation-romania-grants/references/

If you find bugs, spot an outdated figure or want to add new entities, IOCs or scenarios, please open an issue or a pull request. Your input helps strengthen this material for the entire community.

📌 You can find me here: [gabidumitriu.ro](https://gabidumitriu.ro)

## License

This is an open source project under the A Creative Commons (CC) license, meaning it requires Attribution (BY)—giving credit to the creator—and may combine up to three additional conditions: • BY (Attribution): Credit the creator, link to the license, and note any changes made. • SA (ShareAlike): Share any adapted or remixed work under the same (or compatible) license. • NC (NonCommercial): Allow noncommercial use only (no primary monetary compensation or commercial advantage). • ND (NoDerivatives): Share the work only in its original, unadapted form

Built with ❤️ for the Solana community
Funded by a Solana Foundation Grant
