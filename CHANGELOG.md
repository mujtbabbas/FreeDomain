# Changelog

All notable changes to this standalone edition of FreeDomain are documented in this file.

## v1.1.0 — Standalone enhancements (2026-10-20)

- Converted the repository from a fork into a standalone edition with its own history, keeping full upstream credit.
- Added an "About This Standalone Edition" section to `README.md` with the upstream link, base-version provenance, and credit.
- Added `ENHANCEMENTS.md` documenting everything changed in this edition.
- Added `.github/dependabot.yml` for weekly GitHub Actions dependency updates.
- Added markdown linting automation (`.markdownlint.json` and the Markdown check workflow); the check was later scoped via `.markdownlint-cli2.yaml` so it covers this edition's own documentation instead of failing on upstream content.
- Added `.editorconfig` with standard editor settings (UTF-8, LF, 2-space indent).

## v1.0.0 — Upstream baseline (2026-10-20)

- Clean standalone baseline of [DigitalPlatDev/FreeDomain](https://github.com/DigitalPlatDev/FreeDomain) at upstream commit `9c7c54110705760267b07b6e6a6d406d1172a1bf` (upstream HEAD dated 2026-08-12).
- Fork history severed; all files and the AGPL-3.0 licence (`LICENSE`) preserved exactly as-is.
