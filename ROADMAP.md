# Roadmap

## Milestone 0 — Repository foundation
**Status: CONFIGURED**
- [x] Product scope and project principles
- [x] Master prompt for AI collaborators
- [x] Initial data schemas and AI prompts
- [x] Workflow, security, and testing documentation

## Milestone 1 — Accounts and database
**Status: PLANNED**
- [ ] Create private GitHub repository
- [ ] Create Airtable base and tables
- [ ] Create a Google Drive project folder
- [ ] Create Telegram notification destination (optional)
- [ ] Add one authorized sample source and permission reference

**Exit criteria:** one authorized source and one test recording are registered in Airtable.

## Milestone 2 — Manual proof of concept
**Status: PLANNED**
- [ ] Upload authorized sample recording to chosen clipping tool
- [ ] Generate candidate clips
- [ ] Review captions, timing, context, and attribution
- [ ] Store metadata and previews
- [ ] Record actual processing time and cost

**Exit criteria:** at least three candidate clips are reviewed successfully.

## Milestone 3 — No-code automation
**Status: PLANNED**
- [ ] Build Make scenario for new authorized media
- [ ] Trigger clipping workflow using a supported integration
- [ ] Save output and metadata
- [ ] Create Airtable review records
- [ ] Send notification
- [ ] Add retries and duplicate protection

**Exit criteria:** an authorized sample can pass through the workflow without manual data copying, apart from human approval.

## Milestone 4 — Approval and publishing
**Status: PLANNED**
- [ ] Implement approve/reject/request-edit states
- [ ] Verify permission and destination before publishing
- [ ] Connect one authorized social account
- [ ] Test publishing with a private/unlisted or otherwise safe test where supported
- [ ] Audit decision and publication result

**Exit criteria:** only approved, permitted clips can be published.

## Milestone 5 — Live source support
**Status: PLANNED**
- [ ] Identify creator-authorized live feed or recording workflow
- [ ] Verify platform terms and API capabilities
- [ ] Test live segment capture with permission
- [ ] Add monitoring and health alerts
- [ ] Measure compute/storage costs

**Exit criteria:** an authorized live source can produce reviewable clips reliably.

## Milestone 6 — Scale and analytics
**Status: PLANNED**
- [ ] Add more authorized creators
- [ ] Add performance metrics
- [ ] Tune editorial scoring using actual outcomes
- [ ] Add usage and cost limits
- [ ] Document operational playbook
