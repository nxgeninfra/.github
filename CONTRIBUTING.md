# Contributing to nxgeninfra

Thanks for your interest in contributing to open compute specifications.

This guide applies to all repositories under the [github.com/nxgeninfra](https://github.com/nxgeninfra) organization.

## Current Status

The GPU Instance Specification (GIS) is live at v1.0. We welcome contributions to the spec, examples, and documentation.

## How to Contribute

### Spec Contributions (gis-spec)

The GIS specification is open under CC BY 4.0. You can:

- 🐛 Report issues with the spec (ambiguities, missing fields, edge cases)
- 💡 Propose new fields or spec extensions via RFC
- 📖 Improve spec documentation and examples
- 🔧 Submit example GIS documents for providers we haven't covered
- ✅ Validate existing GIS documents against real provider data

### Provider Data

Know a GPU cloud provider we haven't covered? Open a [Provider Request](https://github.com/nxgeninfra/.github/issues/new?template=provider_request.md) issue with:
- Provider name and website
- GPU models offered
- Direct link to pricing page

### What We're NOT Accepting

- Changes to private repositories (site, data pipeline, tools)
- Spec changes that break backwards compatibility without major version bump
- Provider-specific fields that don't generalize across providers
- Fields that fewer than 50% of providers can populate

## Getting Started

1. Fork the relevant repository
2. Create a branch: `git checkout -b improve/spec-field-name`
3. Make your changes
4. Commit using conventional commits (see below)
5. Push and open a Pull Request

## Commit Convention

We use [Conventional Commits](https://www.conventionalcommits.org/):

```
type(scope): description

spec(gpu): add interconnect field to gpu object
schema(v1): update required fields validation
example(coreweave): add CoreWeave H100 SXM GIS document
docs(readme): clarify billing_granularity field
fix(schema): correct vram_gb type to number
```

Types: `spec`, `schema`, `example`, `docs`, `fix`, `chore`

## What Makes a Good Spec Contribution

1. **Solves a real problem** — Provider X can't be described with current fields
2. **Backwards compatible** — Doesn't break existing GIS documents
3. **Includes an example** — Shows the change in action with real data
4. **Minimal** — Every field must earn its place (80%+ of providers can populate it)
5. **Generalizable** — Works across providers, not specific to one

## Code Style (for tooling repos)

- TypeScript strict mode
- Prettier for formatting
- ESLint for linting

## Review Process

1. All spec changes require at least one review
2. Schema changes must include updated examples that validate
3. Breaking changes require a major version bump and migration guide

---

## Contact

| Channel | Address |
|---------|---------|
| General questions | [hello@computespec.dev](mailto:hello@computespec.dev) |
| Spec feedback | [spec@computespec.dev](mailto:spec@computespec.dev) |
| Twitter | [@nxgeninfra](https://x.com/nxgeninfra) |
