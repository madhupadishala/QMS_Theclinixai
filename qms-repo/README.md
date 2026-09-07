# ClinixAI QMS

Quality Management System for ClinixAI — controlled SOPs, training records, and
approved quality records.

## Structure

- `docs/sop/` — Controlled SOPs (Standard Operating Procedures)
- `docs/policy/` — Approved quality policies
- `docs/records/` — Approved quality records (audit trail, CAPA, etc.)
- `training/` — Required training / read-and-understand tasks
- `.github/workflows/` — Automation (e.g. Lark notification triggers)

## Document control rules

1. No document is "approved" until it's merged to `main` via a reviewed pull request.
2. Every SOP must have a version number and effective date in its filename: `SOP-001-v1.0-effective-2026-09-07.md`
3. Draft/working documents belong on a branch, never on `main`.
4. This repo currently holds no PAN, Aadhaar, bank, or personal employee data — that lives in HRM only.

## Status

- [ ] Repo set to private (currently public by team decision, pending)
- [ ] First SOP template added
- [ ] Branch protection enabled on `main`
- [ ] Lark QMS app linked to qms.theclinixai.com
- [ ] Read-only doc portal deployed (Vercel)
