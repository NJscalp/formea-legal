# Formea — legal and release preparation

**Draft. Not yet suitable for App Store submission.** The provider must supply its legal name, postal address, country and public contact email. The documents describe the current source code, not hypothetical future analytics or cloud services.

## Pages

- `site/privacy.html`: privacy policy, local fitness data, Apple purchases, backups, email support and GitHub hosting.
- `site/terms.html`: membership conditions with Apple's Standard EULA, billing, cancellation and general fitness expectations.
- `site/support.html`: contact and troubleshooting.
- `site/index.html`: public information hub.

Edit `provider.json`, then run `python3 build.py --release`. This command refuses missing provider details. Preview locally at `/legal/site/` on the Formea development server. No external fonts, scripts, analytics or contact form are included.

## GitHub Pages publication

The repository is staged privately until the provider details are supplied. Intended repository: `NJscalp/formea-legal`; intended public base URL: `https://njscalp.github.io/formea-legal/`. These are intended URLs, not verified live links.

Once provider details are complete, rebuild with `--release`, commit the completed pages and make the repository public. Enable GitHub Pages with GitHub Actions and run the included manual deployment workflow. Check all public URLs without authentication before adding them to the iOS app and App Store Connect. Do not submit draft pages.

Only legal-site content and release instructions belong in this repository. No Swift source, user state, screenshots, credentials or app assets are included.

## App Store materials

See `release/` for the privacy data map, submission checklist, store copy and review notes. Several release blockers remain: movement demonstrations, professional content review, live subscription configuration/testing, verified contact pages, and asset rights. A privacy policy alone cannot make the current prototype release-ready or guarantee Apple approval.
