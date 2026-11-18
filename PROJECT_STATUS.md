# Project Status

**Project:** ClipHunter AI  
**Version:** 0.1.0 — starter repository  
**Last updated:** 2026-11-18  
**Overall status:** FOUNDATION DOCUMENTATION PREPARED

## Status legend

- `PLANNED` — designed but not configured.
- `CONFIGURED` — set up but not yet validated end-to-end.
- `TESTED` — passed a documented test.
- `DEPLOYED` — running in the intended environment.

## Workstream status

| Workstream | Status | Notes |
|---|---|---|
| Product definition | CONFIGURED | Starter requirements documented |
| Repository structure | CONFIGURED | Starter files generated |
| Rights and permission model | CONFIGURED | Permission-first rules documented |
| Data schemas | CONFIGURED | JSON schemas included |
| AI prompts | CONFIGURED | Initial prompt templates included |
| Airtable base | PLANNED | Must be created in user's account |
| Make scenarios | PLANNED | Blueprint design documented; no live credentials |
| OpusClip integration | PLANNED | Verify current input/API options and terms |
| Authorized source ingestion | PLANNED | Requires creator-authorized footage/feed |
| Clip generation | PLANNED | Test with authorized sample footage |
| Approval dashboard | PLANNED | Airtable implementation pending |
| Notifications | PLANNED | Telegram connection pending |
| Publishing | PLANNED | Disabled until permissions and approval gate tested |

## Decisions made

1. No-code-first with AI-generated code for gaps.
2. Make.com, Airtable, Google Drive, Telegram, and an AI clipping service are candidate tools, not yet connected.
3. Start with free tiers and authorized sample footage.
4. Every clip starts in `PENDING_REVIEW`.
5. No automatic publishing without explicit human approval.
6. Famous streamer channels are research targets only; no permission is assumed.

## Blockers

- User must create/connect required service accounts.
- Need an authorized test recording or creator-provided footage.
- Need to verify current product capabilities, API access, pricing, and terms before selecting integrations.
- Need a permission record defining allowed processing and publishing destinations.

## Next action

Create a private GitHub repository named `ClipHunter-AI` and upload this starter package. Then proceed to the Airtable setup guide in `docs/DEPLOYMENT.md`.
