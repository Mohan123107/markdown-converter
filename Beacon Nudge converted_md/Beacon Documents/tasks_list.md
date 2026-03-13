# Beacon Dev Team — Task List

> **Last Updated:** 2026-02-16
> **Branch:** dev
> **Developers:** Dev 1 (Syed), Dev 2 (TBD), Dev 3 (TBD)

---

## Developer 1 — XDEX Integration & Testing (Syed)

XDEX integration code is ~95% complete (QuickBooks + Oracle CC&B). Focus is on **verification, edge cases, and E2E test coverage**.

| # | Task | Status | Priority | Notes |
|---|------|--------|----------|-------|
| 1.1 | Test and verify Google and Microsoft Auth works. We only support passwordless, Google, and Microsoft auth. | Pending | P0 | OAuth callback flow, JWT token issuance, session persistence |
| 1.2 | Verify QuickBooks OAuth flow end-to-end (initiate auth, callback, token storage, refresh) | Pending | P0 | Endpoint: `POST /api/xdex/quickbooks/initiate-auth` |
| 1.3 | Verify QuickBooks customer sync maps correctly to `contacts` table | Pending | P0 | Endpoint: `POST /api/xdex/quickbooks/sync-customers` |
| 1.4 | Verify QuickBooks invoice sync maps correctly to `erp_invoices` table | Pending | P0 | Endpoint: `POST /api/xdex/quickbooks/sync-invoices` |
| 1.5 | Verify Oracle CC&B credential management and health check | Pending | P1 | Endpoint: `POST /api/xdex/oracle-ccb/set-credentials`, `test-connection` |
| 1.6 | Verify Oracle CC&B customer sync with deduplication guards (`ccbAccountId`, `ccbPersonId`) | Pending | P1 | Endpoint: `POST /api/xdex/oracle-ccb/sync-customers` |
| 1.7 | Test XDEX multi-tenant isolation — ensure tenant A cannot access tenant B data | Pending | P0 | Per-tenant XDEX API keys in admin settings |
| 1.8 | Test ERP Settings page (`/settings/erp`) — XDEX badge, credential UI, connection test buttons | Pending | P1 | Frontend: `apps/web/src/pages/ErpSettings.js` |
| 1.9 | Test onboarding Step 3 — ERP system selection with XDEX-ready badges | Pending | P1 | Frontend: `apps/web/src/pages/JareisOnboarding.tsx` |
| 1.10 | Write E2E Playwright test for XDEX QuickBooks sync flow | Pending | P2 | Add to `apps/web/e2e/` |
| 1.11 | Document any XDEX sandbox limitations and update `docs/XDEX_integration.md` | Pending | P2 | Sandbox: `https://api.xdex-sbx.tilli.pro` |

**Key Files:**
- `apps/api/src/routes/xdex.routes.ts` (970 lines — all XDEX endpoints)
- `apps/web/src/pages/ErpSettings.js`
- `docs/XDEX_integration.md`

---

## Developer 2 — Nudge Integration & Messaging

Nudge messaging integration is complete but needs **testing across all channels and verification of webhook processing**.

| # | Task | Status | Priority | Notes |
|---|------|--------|----------|-------|
| 2.1 | Test passwordless OTP login flow — Nudge SMS delivery, OTP verification, JWT issuance | Pending | P0 | Route: `apps/api/src/routes/auth.routes.ts` |
| 2.2 | Test passwordless OTP with email channel (not just SMS) | Pending | P0 | Nudge client supports SMS + Email |
| 2.3 | Verify Nudge webhook signature verification (SHA256) works in all environments | Pending | P0 | File: `apps/api/src/integrations/nudge/notifications.ts` |
| 2.4 | Test marketing campaign approval reminder emails via Nudge | Pending | P1 | Service: `notification-stats.service.ts` |
| 2.5 | Test billing notifications — payment reminders, overdue alerts | Pending | P1 | Service: `utility-nudges.service.ts` |
| 2.6 | Test workflow `send_message` step — SMS, email, WhatsApp channels | Pending | P1 | Workflow engine step type |
| 2.7 | Test `notify_agent` workflow step — agent notification delivery | Pending | P1 | Workflow engine step type |
| 2.8 | Verify Nudge delivery logs and analytics (`nudge-logs.service.ts`) | Pending | P1 | Delivery/click tracking |
| 2.9 | Test utility nudges — outage alerts, bill due reminders | Pending | P2 | Service: `utility-nudges.service.ts` |
| 2.10 | Verify Nudge `v1` vs `v2` send endpoint configuration works correctly | Pending | P2 | Env: `NUDGE_SEND_ENDPOINT=/v2/Nudge/Send` |
| 2.11 | Write E2E test for full OTP login → dashboard flow (extend `passwordless-login.spec.ts`) | Pending | P2 | Existing test may need real Nudge integration |
| 2.12 | Test omnichannel console — thread view, composer, template approvals | Pending | P1 | Files: `apps/web/src/components/omnichannel/` |

**Key Files:**
- `apps/api/src/integrations/nudge/client.ts` (Nudge API client)
- `apps/api/src/integrations/nudge/notifications.ts` (webhook verification)
- `apps/api/src/services/nudge-logs.service.ts`
- `apps/api/src/services/utility-nudges.service.ts`
- `apps/api/src/services/notification-stats.service.ts`

**Environment:**
```
NUDGE_API_URL=https://app.nudge.net/api
NUDGE_SEND_API_URL=https://app.nudge.net/api
NUDGE_SEND_ENDPOINT=/v2/Nudge/Send
NUDGE_FROM_SMS=18448443464
NUDGE_FROM_EMAIL=notification@nudge.net
```

---

## Developer 3 — End-to-End Testing & Quality

Beacon has 8 E2E test suites + API smoke tests but **no unit tests and several coverage gaps**. This developer owns test infrastructure and overall quality.

| # | Task | Status | Priority | Notes |
|---|------|--------|----------|-------|
| 3.1 | Run all existing E2E tests and fix any failures | Pending | P0 | `pnpm -C apps/web e2e` (8 suites) |
| 3.2 | Run all API smoke tests and fix any failures | Pending | P0 | `pnpm -C apps/api test:marketing`, `test:finance:tb-smoke` |
| 3.3 | Run finance smoke test — invoice, payment, bill, ledger posting via TigerBeetle | Pending | P0 | `pnpm -C apps/api test:finance:tb-smoke` |
| 3.4 | Run admin auth guardrails smoke test | Pending | P0 | `pnpm -C apps/api test:admin-auth` |
| 3.5 | Run workflow TODO actions smoke test | Pending | P0 | Tests: create_task, create_ticket, update_record, assign_agent, notify_agent, deflection |
| 3.6 | Run CCB golden replay + schema drift tests | Pending | P1 | `pnpm -C apps/api test:ccb:golden`, `test:ccb:drift` |
| 3.7 | Set up Vitest for unit tests (API services layer) | Pending | P1 | No unit test framework exists today |
| 3.8 | Write unit tests for `ledger.service.ts` — TigerBeetle posting logic | Pending | P1 | Critical financial logic |
| 3.9 | Write unit tests for `jareis-assistant.service.ts` — rule-based suggestions | Pending | P2 | Validate risk detection, sentiment, escalation logic |
| 3.10 | Test TilliPay payment flow — card + ACH endpoints | Pending | P1 | Routes: `/api/tillipay/card`, `/api/tillipay/ach` |
| 3.11 | Test customer invoice lifecycle: create, add line items, send, record payment, void | Pending | P1 | Routes: `/api/customer-invoices/*` |
| 3.12 | Test vendor bill lifecycle: create, add line items, approve, pay, void | Pending | P1 | Routes: `/api/vendor-bills/*` |
| 3.13 | Test ledger reporting endpoints — balance sheet, income statement, journal entries | Pending | P2 | Routes: `/api/ledger/*` |
| 3.14 | Verify multi-tenant data isolation across all major entities | Pending | P0 | Contacts, invoices, bills, tickets, workflows |
| 3.15 | Apply finance migration to staging and run repair/audit scripts | Pending | P0 | Migration: `packages/db/drizzle/0003_curved_drax.sql` |

**Test Commands:**
```bash
pnpm test                                    # All tests
pnpm -C apps/web e2e                         # Playwright E2E (8 suites)
pnpm -C apps/web e2e:real-smoke              # Real browser smoke
pnpm -C apps/api test:marketing              # Marketing approval tests
pnpm -C apps/api test:finance:tb-smoke       # Finance/TigerBeetle smoke
pnpm -C apps/api test:approvals:api          # Approval email tests
pnpm db:audit                                # Finance guardrails audit (if script exists)
```

**Key Files:**
- `apps/web/e2e/*.spec.ts` (8 E2E test suites)
- `apps/api/src/scripts/*-test.ts` (API smoke tests)
- `packages/db/src/audit-finance-guardrails.ts`
- `packages/db/src/repair-finance-guardrails.ts`
- `.github/workflows/` (3 CI pipelines)

---

## Cross-Team — Known Gaps (Assign as capacity allows)

| # | Task | Owner | Status | Priority | Notes |
|---|------|-------|--------|----------|-------|
| X.1 | Complete GitHub OAuth server-side token exchange | TBD | Pending | P2 | Auth route exists, GitHub API call incomplete |
| X.2 | Connect LLM (OpenAI/Anthropic) to Jareis ticket assistant | TBD | Pending | P1 | Currently rule-based only; placeholder in `jareis-assistant.service.ts` |
| X.3 | Implement Contact Center call transfers (warm/cold) | TBD | Pending | P2 | AWS Connect Streams integration |
| X.4 | Implement call recording playback UI | TBD | Pending | P2 | S3 presigned URLs + audio player component |
| X.5 | Navigation redesign (collapsible sidebar, contextual tabs, mobile) | TBD | Pending | P2 | Spec: `docs/Beacon_Nav_2026.md` |
| X.6 | Payment link generation via TilliPay | TBD | Pending | P2 | Route skeleton exists, not wired |

---

## Status Legend

- **P0** — Must complete before staging/production
- **P1** — Required for launch readiness
- **P2** — Important but can follow initial launch
- **Pending** — Not started
- **In Progress** — Actively being worked on
- **Done** — Verified complete
