# Formea — legal and release preparation

**Release preparation; app submission blockers remain.** Provider: Normann Jungbauer, under the Formea brand. Contact: clavic.ai.app@gmail.com. The provider has not supplied a postal address or country; jurisdiction-specific business/trader disclosures still need those real details. No address is invented. The documents describe the current source code, not hypothetical future analytics or cloud services.

## Pages

- `site/privacy.html`: privacy policy, local fitness data, Apple purchases, backups, email support and GitHub hosting.
- `site/terms.html`: membership conditions with Apple's Standard EULA, billing, cancellation and general fitness expectations.
- `site/support.html`: contact and troubleshooting.
- `site/index.html`: public information hub.

Edit `provider.json`, then run `python3 build.py --release`. This command refuses missing legal identity, contact email or website URL. Postal address and country are optional site fields until supplied; this does not certify compliance with jurisdiction-specific provider disclosures. Preview locally at `/legal/site/` on the Formea development server. No external fonts, scripts, analytics or contact form are included.

## GitHub Pages publication

Repository: `NJscalp/formea-legal`; public base URL after deployment: `https://njscalp.github.io/formea-legal/`.

The public policy and support pages identify the actual provider and contact email. GitHub Pages uses the included workflow. Check all public URLs without authentication before adding them to App Store Connect. Complete postal/trader information before submission wherever applicable; this repository cannot infer the provider's business jurisdiction.

Public branding is **© 2026 Formea**, with **clavic.ai.app@gmail.com** as the contact. The actual legal provider, **Normann Jungbauer**, appears once per page in a readable provider section in the footer. The privacy policy and membership terms link directly to that section. Public pages contain no telephone number. The native app interface uses Formea and the support email, without the provider's personal name. Footer placement is a presentation choice; the legal identity remains public and is not anonymous or concealed from readers.

Only legal-site content and release instructions belong in this repository. No Swift source, user state, screenshots, credentials or app assets are included.

## App Store materials

See `release/` for the privacy data map, submission checklist, store copy and review notes. Several release blockers remain: movement demonstrations, professional content review, live subscription configuration/testing, verified contact pages, and asset rights. A privacy policy alone cannot make the current prototype release-ready or guarantee Apple approval.
