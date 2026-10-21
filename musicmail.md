# MusicMail

MusicMail is a web application for independent musicians to discover industry
contacts, organise a private professional network, plan events and manage
follow-ups. It includes an optional Gmail sending integration.

**Next.js · React · TypeScript · PostgreSQL · Supabase · Vitest · Playwright**

## Engineering milestone — Phase 1: upgrade safety

The challenge was to extend a working application while preserving existing
accounts, private CRM records and established workflows.

I consolidated the next application version, documented the deployed baseline,
and added repeatable database upgrade rehearsals using synthetic data. Tests
check existing account access, stable references, saved filters, event records,
appearance preferences, exports and account deletion after an upgrade. Reciprocal
isolation tests check that separate workspaces retain their own private records.

Validation combines TypeScript and lint checks, unit tests, PostgreSQL integration
tests, browser workflows and real isolated authentication services. Dependency
and secret checks accompany the release. Local regression evidence is kept
separate from production deployment claims.

The trade-off was to extend established structures and retain compatibility,
rather than introduce a parallel implementation. Reproducible fixtures make
upgrade safety reviewable without copying customer data.

This milestone is a private engineering release; it does not claim a production
rollout of the new version. The application source remains proprietary. This
standalone case study contains no production code, schema, internal algorithms,
credentials, customer data or internal operational documents.

[MusicMail](https://app.musicmailapp.uk)
