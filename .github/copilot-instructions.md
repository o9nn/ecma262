# Copilot Instructions for ECMA-262 Repository

This guide provides essential knowledge for AI coding agents working in the ECMA-262 specification repo. Follow these conventions and workflows for productive contributions.

## Project Overview
- This repo contains the source for the ECMAScript Language Specification (`spec.html`).
- Output is generated via [ecmarkup](https://github.com/tc39/ecmarkup) into the `out/` directory.
- The `biblio/` package provides a machine-readable bibliography for spec tooling.

## Key Workflows
- **Setup:** Run `npm install` after cloning.
- **Build Spec:**
  - `npm run build` (main build)
  - `npm run watch` (continuous build)
  - Output appears in `out/`.
- **Clean Output:** `npm run clean` removes the `out/` directory.
- **PDF Generation:** `npm run pdf` builds a printable spec PDF in `out/ECMA-262.pdf`.
- **Biblio Publish:** Run `scripts/publish-biblio.sh` to update and publish the bibliography package.
- **Spellcheck:** Use `scripts/spellcheck.mjs <base-ref>` to check for typos in `spec.html`.
- **Deploy to GitHub Pages:** Use `scripts/deploy-github-pages.sh` (see script for PR-specific options).

## Commit Message Conventions
- All commit messages must start with one of: `Normative:`, `Editorial:`, `Meta:`, `Layering:`
- All commits must end with ` (#123)` where `123` is the PR number.
- Use `scripts/check-commit.js` to validate commit messages.

## Directory Structure
- `spec.html`: Main specification source.
- `biblio/`: Bibliography package, auto-updated and published to npm.
- `scripts/`: Utility scripts for build, validation, deployment, and publishing.
- `img/`: Images used in the spec.

## External Dependencies
- Uses `ecmarkup` for spec processing and output.
- Bibliography consumers should pin exact versions due to instability.

## Patterns & Conventions
- Editorial and normative changes are tracked via commit prefixes.
- PRs and proposals follow the [TC39 process](https://tc39.es/process-document/).
- For contributing new proposals, see `CONTRIBUTING.md`.

## References
- [README.md](../README.md): Project overview and links
- [biblio/README.md](../biblio/README.md): Bibliography details
- [CONTRIBUTING.md](../CONTRIBUTING.md): Contribution guidelines

---

If any section is unclear or missing, please provide feedback for improvement.
