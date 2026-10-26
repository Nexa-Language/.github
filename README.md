# Nexa organization profile

This repository maintains the [Nexa-Language organization homepage](https://github.com/Nexa-Language), shared contribution guidance, and community templates.

- [Organization profile](profile/README.md)
- [Contribution guide](CONTRIBUTING.md)
- [Code of conduct](CODE_OF_CONDUCT.md)

The profile uses the existing Nexa mark, graphite and paper surfaces, restrained blue accents, and native GitHub Markdown. Light and dark SVG banners live in `profile/assets/`. They contain no external font requests, scripts, or animations; all navigation and explanatory content remains accessible in Markdown.

The profile targets Nexa 3.0.0 Open Programs and preserves the documented 2.4 compatibility boundary. Its example demonstrates an open goal; `nexa check` validates the source offline, while resolution needs a provider, checks, a budget, and the documented OCI environment.

Before publishing a profile change, verify repository links and documentation routes, check the complete `.nx` example with the pinned Nexa release, parse both SVGs, and inspect the profile at desktop and mobile widths. Publish the matching 3.0 documentation and tooling before the profile that links to them. Banner URLs intentionally target this repository's default branch and become available when the assets are merged.

Suggested organization description: **An agent-native language and runtime. Built for people and models.**

Suggested pinned repositories: **Nexa**, **Nexa-Code**, **Nexa-extension**, **Nexa-docs**, followed by two research projects selected by maintainers. Organization settings and pinned repositories are managed separately from this source change.
