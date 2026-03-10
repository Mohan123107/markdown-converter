## Sheet: Follow up list

| List to Follow up | Date | owner | followup Status | comments |  |
| --- | --- | --- | --- | --- | --- |
| Access to Tilli Claude accounts  for amit , Syed , Suryakanth | 2026-02-09 00:00:00 | Sushmitha | Done | sent the email |  |
| infra to work with hassan , to assign the github accounts for claude | 2026-02-09 00:00:00 | Sushmitha | Done | sent the email |  |
| once 1 , 2 is done , there is a docx folder in Git , Task list will be there , all the tasks will be given by Ali in the Task List ( updates can be found there ) | 2026-02-10 00:00:00 | Ali | Done | task list given out |  |
| Sushmitha to schedule a call - daily at 10  am EST | 2026-02-09 00:00:00 | Sushmitha | Done |  |  |
| Amit , Syed , Suryakanth to walk Ali through on what they have built till now for 5 mins each with AI. | 2026-02-10 00:00:00 | Sushmitha | Done | scheduled a demo ,  from the team |  |
| Draft Beacon AI development policy | 2026-02-11 00:00:00 | Dev Team | in progress | to merge as the single doc , et : 18-feb |  |
| Explore AI website builder within Beacon |  | Suryakant | inprogress | working on this |  |
| Follow up on Claude/GitHub access | 2026-02-10 00:00:00 | Sushmitha | Done | Access Provided |  |
| Review & harden existing Beacon components |  | Amit |  |  |  |
| Define sprint documentation & review process | 2026-02-17 00:00:00 | sushmitha | in progress |  |  |
| Claude Code Console Dev Access | 2026-02-13 00:00:00 | Infra | Done | followup call on 18-feb |  |
| Tilli / Google Partnership | 2026-02-11 00:00:00 | Sushmitha | Done | meeting invite sent to the team |  |
| work with Infra to get Dev built. | 2026-02-16 00:00:00 | Ali | Done |  |  |
| Allocate this one to the VSCode console for the team - Amit, Syed and Suryakant. | 2026-02-16 00:00:00 | Infra |  | worked for Amit , need to take confirmation from Surya and Syed |  |
| Tilli Beacon API Keys for AWS | 2026-02-16 00:00:00 | Ali | done | infra updated the requested autorization |  |
| AWS Dev ECS | 2026-02-16 00:00:00 | Infra |  | need to clarify with Ali | infra is working on it - to go with Node not the ubuntu version - Node Alpine |
| Mobile apllication access to Suryakanth | 2026-02-17 00:00:00 | sushmitha |  | sent out an email |  |
| TilliArc Endpoints for PDF | 2026-02-17 00:00:00 | Raja |  | followup email to raja sir |  |
|  |  |  |  |  |  |
|  |  |  |  |  |  |
| Follow-up Item | Context from Discussion | Action Required | Priority | Target |  |
| Create Detailed Project Plan | Ali asked for Sprint / Project plan | Convert task list into structured project plan | High | Immediate | inprogress |
| Create Jira Project & Tasks | Excel draft mentioned | Move task list into Jira with proper breakdown | High | This week |  |
| Get Estimates from Dev Team | Required before planning | Collect effort estimates (Syed, Amit, Surya, Hassan) | High | Before sprint finalization |  |
| Align Tasks with Ali’s Original Email | Ali asked to review original assignment list | Re-map tasks to correct owners (Beacon / Marketing / XDEX / Monay) | High | Immediate |  |
| Define MVP Scope Clearly (Beacon) | Multiple parallel discussions happening | Document MVP: ERP Sync, Financial Sync, Marketing Integration | High | Before next review |  |
| Track Access & Environment Issues | Devs had revoked access issue | Ensure infra stability & confirm access for all devs | Medium | Ongoing |  |
| Daily Tracker Circulation | Multiple complex modules discussed | Share structured daily tracker with status updates | High | Daily |  |

## Sheet: Claude task list

| Beacon Dev Team — Task List |  |  |  |  |  |  |  |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Last Updated: 2026-02-16   \|   Branch: dev   \|   Developers: Syed (Dev 1), TBD (Dev 2), TBD (Dev 3) |  |  |  |  |  |  |  |
| Task ID | Task Description | Responsible Person | Category | Status | Priority | Notes | 2026-02-18 00:00:00 |
| Developer 1 — XDEX Integration & Testing (Syed) |  |  |  |  |  |  |  |
| 1.1 | Test and verify Google and Microsoft Auth works (passwordless, Google, Microsoft auth only) | Syed | Dev 1 – Syed | Pending | P0 | OAuth callback flow, JWT token issuance, session persistence |  |
| 1.2 | Verify QuickBooks OAuth flow end-to-end (initiate auth, callback, token storage, refresh) | Syed | Dev 1 – Syed | Pending | P0 | Endpoint: POST /api/xdex/quickbooks/initiate-auth |  |
| 1.3 | Verify QuickBooks customer sync maps correctly to contacts table | Syed | Dev 1 – Syed | Pending | P0 | Endpoint: POST /api/xdex/quickbooks/sync-customers |  |
| 1.4 | Verify QuickBooks invoice sync maps correctly to erp_invoices table | Syed | Dev 1 – Syed | Pending | P0 | Endpoint: POST /api/xdex/quickbooks/sync-invoices |  |
| 1.5 | Verify Oracle CC&B credential management and health check | Syed | Dev 1 – Syed | Pending | P1 | Endpoint: POST /api/xdex/oracle-ccb/set-credentials, test-connection |  |
| 1.6 | Verify Oracle CC&B customer sync with deduplication guards (ccbAccountId, ccbPersonId) | Syed | Dev 1 – Syed | Pending | P1 | Endpoint: POST /api/xdex/oracle-ccb/sync-customers |  |
| 1.7 | Test XDEX multi-tenant isolation — ensure tenant A cannot access tenant B data | Syed | Dev 1 – Syed | Pending | P0 | Per-tenant XDEX API keys in admin settings |  |
| 1.8 | Test ERP Settings page (/settings/erp) — XDEX badge, credential UI, connection test buttons | Syed | Dev 1 – Syed | Pending | P1 | Frontend: apps/web/src/pages/ErpSettings.js |  |
| 1.9 | Test onboarding Step 3 — ERP system selection with XDEX-ready badges | Syed | Dev 1 – Syed | Pending | P1 | Frontend: apps/web/src/pages/JareisOnboarding.tsx |  |
| 1.1 | Write E2E Playwright test for XDEX QuickBooks sync flow | Syed | Dev 1 – Syed | Pending | P2 | Add to apps/web/e2e/ |  |
| 1.11 | Document XDEX sandbox limitations and update docs/XDEX_integration.md | Syed | Dev 1 – Syed | Pending | P2 | Sandbox: https://api.xdex-sbx.tilli.pro |  |
| Developer 2 — Nudge Integration & Messaging |  |  |  |  |  |  | Hassan |
| 2.1 | Test passwordless OTP login flow — Nudge SMS delivery, OTP verification, JWT issuance | TBD | Dev 2 – TBD | Pending | P0 | Route: apps/api/src/routes/auth.routes.ts |  |
| 2.2 | Test passwordless OTP with email channel (not just SMS) | TBD | Dev 2 – TBD | Pending | P0 | Nudge client supports SMS + Email |  |
| 2.3 | Verify Nudge webhook signature verification (SHA256) works in all environments | TBD | Dev 2 – TBD | Pending | P0 | File: apps/api/src/integrations/nudge/notifications.ts |  |
| 2.4 | Test marketing campaign approval reminder emails via Nudge | TBD | Dev 2 – TBD | Pending | P1 | Service: notification-stats.service.ts |  |
| 2.5 | Test billing notifications — payment reminders, overdue alerts | TBD | Dev 2 – TBD | Pending | P1 | Service: utility-nudges.service.ts |  |
| 2.6 | Test workflow send_message step — SMS, email, WhatsApp channels | TBD | Dev 2 – TBD | Pending | P1 | Workflow engine step type |  |
| 2.7 | Test notify_agent workflow step — agent notification delivery | TBD | Dev 2 – TBD | Pending | P1 | Workflow engine step type |  |
| 2.8 | Verify Nudge delivery logs and analytics (nudge-logs.service.ts) | TBD | Dev 2 – TBD | Pending | P1 | Delivery/click tracking |  |
| 2.9 | Test utility nudges — outage alerts, bill due reminders | TBD | Dev 2 – TBD | Pending | P2 | Service: utility-nudges.service.ts |  |
| 2.1 | Verify Nudge v1 vs v2 send endpoint configuration works correctly | TBD | Dev 2 – TBD | Pending | P2 | Env: NUDGE_SEND_ENDPOINT=/v2/Nudge/Send |  |
| 2.11 | Write E2E test for full OTP login → dashboard flow | TBD | Dev 2 – TBD | Pending | P2 | Extend passwordless-login.spec.ts; may need real Nudge integration |  |
| 2.12 | Test omnichannel console — thread view, composer, template approvals | TBD | Dev 2 – TBD | Pending | P1 | Files: apps/web/src/components/omnichannel/ |  |
| Developer 3 — End-to-End Testing & Quality |  |  |  |  |  |  | Amit , Syed |
| 3.1 | Run all existing E2E tests and fix any failures | TBD | Dev 3 – TBD | Pending | P0 | pnpm -C apps/web e2e (8 suites) |  |
| 3.2 | Run all API smoke tests and fix any failures | TBD | Dev 3 – TBD | Pending | P0 | pnpm -C apps/api test:marketing, test:finance:tb-smoke |  |
| 3.3 | Run finance smoke test — invoice, payment, bill, ledger posting via TigerBeetle | TBD | Dev 3 – TBD | Pending | P0 | pnpm -C apps/api test:finance:tb-smoke |  |
| 3.4 | Run admin auth guardrails smoke test | TBD | Dev 3 – TBD | Pending | P0 | pnpm -C apps/api test:admin-auth |  |
| 3.5 | Run workflow TODO actions smoke test (create_task, create_ticket, update_record, assign_agent, notify_agent, deflection) | TBD | Dev 3 – TBD | Pending | P0 | Tests: create_task, create_ticket, update_record, assign_agent, notify_agent, deflection |  |
| 3.6 | Run CCB golden replay + schema drift tests | TBD | Dev 3 – TBD | Pending | P1 | pnpm -C apps/api test:ccb:golden, test:ccb:drift |  |
| 3.7 | Set up Vitest for unit tests (API services layer) | TBD | Dev 3 – TBD | Pending | P1 | No unit test framework exists today |  |
| 3.8 | Write unit tests for ledger.service.ts — TigerBeetle posting logic | TBD | Dev 3 – TBD | Pending | P1 | Critical financial logic |  |
| 3.9 | Write unit tests for jareis-assistant.service.ts — rule-based suggestions | TBD | Dev 3 – TBD | Pending | P2 | Validate risk detection, sentiment, escalation logic |  |
| 3.1 | Test TilliPay payment flow — card + ACH endpoints | TBD | Dev 3 – TBD | Pending | P1 | Routes: /api/tillipay/card, /api/tillipay/ach |  |
| 3.11 | Test customer invoice lifecycle: create, add line items, send, record payment, void | TBD | Dev 3 – TBD | Pending | P1 | Routes: /api/customer-invoices/* |  |
| 3.12 | Test vendor bill lifecycle: create, add line items, approve, pay, void | TBD | Dev 3 – TBD | Pending | P1 | Routes: /api/vendor-bills/* |  |
| 3.13 | Test ledger reporting endpoints — balance sheet, income statement, journal entries | TBD | Dev 3 – TBD | Pending | P2 | Routes: /api/ledger/* |  |
| 3.14 | Verify multi-tenant data isolation across all major entities | TBD | Dev 3 – TBD | Pending | P0 | Contacts, invoices, bills, tickets, workflows |  |
| 3.15 | Apply finance migration to staging and run repair/audit scripts | TBD | Dev 3 – TBD | Pending | P0 | Migration: packages/db/drizzle/0003_curved_drax.sql |  |
| Cross-Team — Known Gaps (Assign as capacity allows) |  |  |  |  |  |  |  |
| X.1 | Complete GitHub OAuth server-side token exchange | TBD | Cross-Team | Pending | P2 | Auth route exists, GitHub API call incomplete |  |
| X.2 | Connect LLM (OpenAI/Anthropic) to Jareis ticket assistant | TBD | Cross-Team | Pending | P1 | Currently rule-based only; placeholder in jareis-assistant.service.ts |  |
| X.3 | Implement Contact Center call transfers (warm/cold) | TBD | Cross-Team | Pending | P2 | AWS Connect Streams integration |  |
| X.4 | Implement call recording playback UI | TBD | Cross-Team | Pending | P2 | S3 presigned URLs + audio player component |  |
| X.5 | Navigation redesign (collapsible sidebar, contextual tabs, mobile) | TBD | Cross-Team | Pending | P2 | Spec: docs/Beacon_Nav_2026.md |  |
| X.6 | Payment link generation via TilliPay | TBD | Cross-Team | Pending | P2 | Route skeleton exists, not wired |  |

## Sheet: Legend

| Status / Priority Legend |  |
| --- | --- |
|  |  |
| PRIORITY |  |
| P0 | Must complete before staging / production |
| P1 | Required for launch readiness |
| P2 | Important but can follow initial launch |
|  |  |
| STATUS |  |
| Pending | Not started |
| In Progress | Actively being worked on |
| Done | Verified complete |
|  |  |
| SECTIONS |  |
| Dev 1 – Syed | XDEX Integration & Testing |
| Dev 2 – TBD | Nudge Integration & Messaging |
| Dev 3 – TBD | End-to-End Testing & Quality |
| Cross-Team | Known gaps — assign as capacity allows |

## Sheet: Task List - Ali

| # | Task List | Status - feb 17 | Comments | Status - feb 18 |
| --- | --- | --- | --- | --- |
| 1 | Infra to setup Docker for Postgress, Radis and Tiger beetle in Dev environment. No local installs please. >> Infra | in progress |  |  |
| 2 | AI Policy and Procedure (merge the work of all product teams - Sushmita has the handle on documents from Beacon team) >>  Raja owns this one. | inprogress |  |  |
| 3 | Amit, Syed and Suryakant  - VSCode Claude Console to git - no direct git access >> Work already cut out for them. >> Sushmitha to follow through | Amit : done , syed n surya kanth ro review |  |  |
| 4 | Help on Monay (separate email on that soon) >> Ali to work with Infra tos et up Dev for Monay on Monay Pay AWS. Suryakant to work with Ali on MVP mobile launch. | to work with Suryakanth (pending) need to get the update |  |  |
| 5 | Sriram and Abdul will join me and Hassan -  nudge , Raja - Tilli arc | FYI |  |  |
| 6 | tillipay (payin/payout) integration to Beacon >> Sriram | to work with Sriram |  |  |
| 7 | Regression across all existing flows supported in Beacon >> Amit (Starting marketing hooks to all social media) | amit : in progress , to get the clarification from Ali | Amit to work on social media research -  proposed the idea of Xdex integration |  |
| 8 | XDEX integration to Beacon >> Abdul/Syed | Work on Api key with Xdex configration | to work with adbul -  to sync 3 things [Customers , vendors , employees ],[invoices,bills ,payrolls ,  payments ] , to work with Sriram for the intergration for tilliPay |  |
| 9 | Nudge Integration to Beacon >> Hassan |  |  |  |
| 10 | tilliX (post login), integration to beacon >> Ibrahim |  |  |  |
| 11 | tilliArc Integration to Beacon >> Raj (we load bills and have invoices - i am hoping oto use all documents / statements, etc. into TilliArc - right now direct to S3) |  |  |  |
| 12 | Beacon Admin (Intrastate?) will be centralized to manage tilliX, Nudge, Beacon, tilliPay applications for internal purposes >> Ibrahim & Raja |  |  |  |
| 13 | Target Integration Beacon Testing >> End of Feb (possible?) |  |  |  |
| 14 | Production deployment Mid-March |  |  |  |
| 15 | Beacon Product documentation >> Sravan/Hari, |  |  |  |
| 16 | Pricing and subscription >> Sravan, Shabbir, Ali |  |  |  |
| 17 | Update tillisoftware website >> Hari |  |  |  |

## Sheet: Feb 17

| Beacon – Daily Status Update with MoM |  |  |  |  |  |  |  |  |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Date: 17-Feb-2026 |  |  |  |  |  |  |  |  |
| Project: Beacon |  |  |  |  |  |  |  |  |
| Meeting Type: Daily Sync |  |  |  |  |  |  |  |  |
| # | Task / Topic | Owner | Current Status | Discussion / Update (MoM) | Next Action | Priority | 2026-02-18 00:00:00 | 2026-02-19 00:00:00 |
| 1 | VS Code & Access Setup | Amit, Syed, Suryakant | done | Amit confirmed access working. Others yet to verify. | Syed & Surya to confirm setup replication | High | done |  |
| 2 | XDEX Global API Config (Admin Level) | Syed | In Progress | API key configured at Super Admin. Tenant-level sync failing. | Debug API key usage & refactor config separation (Admin vs Tenant) | High | to look into this | working on onboarding import contacts  -  (bugs indentified while doing the code walkthrough |
| 3 | QuickBooks via XDEX | Syed + Abdul | Issue Identified | Callback issue – appears direct QuickBooks auth instead of XDEX loop. | Abdul to verify callback path & authentication flow | High |  |  |
| 4 | ERP Sync (Customers / Vendors / Employees) | Syed | In Progress | Need generic schema for multiple ERPs (Oracle, QuickBooks, FreshBooks, Xero). | Implement abstraction layer for ERP sync | High |  |  |
| 5 | Financial Sync (Invoices, Bills, Payments, Payroll) | Syed | Pending | MVP requires: Sync Person + Sync Financials (Invoices & Bills minimum). | Prioritize connectivity → then invoice/bill push-back to ERP | High |  |  |
| 6 | Marketing – Social Media Integration (LinkedIn, Google Ads) | Amit | Research Phase | LinkedIn & Google Ads partially integrated. Need unified admin-level integration. | Research best architecture (Aggregator vs Direct) | High | looking into previous imprementation for google | waiting for Linkedin keys , |
| 7 | Marketing Billing Logic | Amit | Not Started | Spend should flow to Enterprise Billing (Admin-controlled). | Design spend tracking + billing mapping | Medium |  |  |
| 8 | Dynamic Multi-Step Form → Marketing Integration | Amit | Not Started | Forms created via Jarvis need to plug into Marketing campaigns. | MVP: Simple dynamic form → campaign linkage | Medium |  |  |
| 9 | Social Media OAuth & Handle Mapping | Amit | Research Required | Users should only provide handle; platform authentication needed securely. | Research OAuth + key management model | High | to look into this |  |
| 10 | TilliPay Integration | Syed + Sriram | Pending | TilliPay currently direct. Needs review for integration alignment. | Validate API keys + confirm working flow | Medium |  |  |
| 11 | Onboarding Flow (ERP Connect During Signup) | Syed | Broken | ERP connection failing during onboarding flow. | Fix XDEX connection during signup stage | High |  |  |
| 12 | Monay Walley(Mobile) | Suryakant + Ali | In Progress | Complex module. Separate 1:1 required. | Schedule detailed walkthrough | Medium | got the git access , started with the code review | got the repo access 2 days  back , looking into login |

## Sheet: Tasks (old)

| Task | Assignee | Assigned Date | 2026-02-12 00:00:00 | 2026-02-13 00:00:00 | 2026-02-17 00:00:00 |
| --- | --- | --- | --- | --- | --- |
| 1) http://localhost:4200/marketing end to end regression (marketing Campaign, onboarding using Dynamic Flow, ending into the Application for review of signed up /applicants - http://localhost:4200/applications, add hooks for all social media channels (R&D needed) | Assign to Amit | 2026-02-11 00:00:00 | working on the setup , connected with Hasaan . | working on marketing survey , to create the show Ali today | to discuss with Ali regarding the flow |
| 2) Integration to XDEX http://localhost:4200/settings/erp - extend support for more then 1 ERPs with one key (e.g. Account Number, or complex - multiple keys mapping capability to be added - first name, last name, service zip code, or billing zip code, etc.), mapping across multiple backends. Use different tenants to test across QB, Oracle CC&B, SAP, etc. | Soheb to work with Abdul | 2026-02-11 00:00:00 | trying to run locally | ran the project locally, connected with adbul for xdex (working on structured approach) | no updates |
| 3) Monay Mobile MVP - regression and thorough testing for end to end issues, and deploying the Monay stack to AWS CI. >> | Suryakant. | 2026-02-11 00:00:00 | to clarify with Ali. | local setup is done , need to get a brief walktrough on monay application | no updates |
