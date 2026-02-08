# Security Policy

This policy applies to all repositories under the [github.com/nxgeninfra](https://github.com/nxgeninfra) organization.

## Reporting a Vulnerability

If you discover a security vulnerability in any nxgeninfra project, please report it responsibly.

**Do NOT:**
- Open a public GitHub issue
- Post about it on social media
- Exploit the vulnerability

**Do:**
- Email [security@computespec.dev](mailto:security@computespec.dev) with subject "SECURITY: [repo-name]"
- Include detailed steps to reproduce
- Give us reasonable time to respond (48 hours)

## What We Consider Security Issues

- XSS, CSRF, or injection vulnerabilities on computespec.dev
- Data exposure or leakage in published packages
- Authentication/authorization bypasses
- Sensitive data in client-side code or logs
- Dependency vulnerabilities (critical/high severity)
- GIS schema validation bypass that could lead to data integrity issues
- Data pipeline credential exposure

## What We Don't Consider Security Issues

- Missing security headers on static pages
- Rate limiting on unauthenticated endpoints (pre-launch)
- Clickjacking on non-sensitive pages
- Theoretical attacks without proof of concept
- Spec ambiguities (file as regular issues, not security reports)

## Response Timeline

| Severity | Acknowledgment | Fix Timeline |
|----------|---------------|-------------|
| Critical | 24 hours | 24-48 hours |
| High | 48 hours | 7 days |
| Medium | 48 hours | 30 days |
| Low | 7 days | Next release |

## Recognition

We appreciate security researchers who help keep our projects safe. We maintain a hall of fame for responsible disclosures.

---

**Security contact:** [security@computespec.dev](mailto:security@computespec.dev)
**General contact:** [hello@computespec.dev](mailto:hello@computespec.dev)
**Website:** [computespec.dev](https://computespec.dev)
**Twitter:** [@nxgeninfra](https://x.com/nxgeninfra)
