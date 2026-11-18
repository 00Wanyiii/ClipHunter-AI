# ClipHunter AI

**A no-code-first, AI-assisted livestream highlight clipping system with human approval before publishing.**

ClipHunter AI is designed to help a creator or clipping operator process **authorized livestream feeds and recordings**, identify compelling moments, generate short-form edits, review them, and publish only after explicit approval.

## Current status

This is a **starter repository and implementation blueprint**, not a deployed service. The included workflows, schemas, prompts, and setup guides establish the project foundation. External accounts, API credentials, creator permissions, and Make/OpusClip integrations must still be configured and tested.

See [`PROJECT_STATUS.md`](PROJECT_STATUS.md) for the current state and [`ROADMAP.md`](ROADMAP.md) for milestones.

## Core principles

1. **Permission first:** a public stream URL does not automatically grant permission to record, download, edit, or republish it.
2. **Human approval:** every candidate clip starts as `PENDING_REVIEW`. Publishing is blocked until an authorized human approves it.
3. **No platform circumvention:** do not bypass access controls, DRM, paywalls, private streams, rate limits, or platform restrictions.
4. **Traceability:** retain source URL, creator, permission evidence/reference, timestamps, processing history, and publication status.
5. **No fabricated claims:** distinguish planned, configured, tested, and deployed capabilities.
6. **Cost control:** begin with free tiers and sample footage; upgrade only when measured usage justifies it.

## Starter stack

| Layer | Initial choice | Alternatives |
|---|---|---|
| Automation | Make.com | n8n, Zapier |
| AI clipping/editing | OpusClip | Eklipse, Streamladder, approved custom pipeline |
| Database / review queue | Airtable | Google Sheets, Supabase |
| Media storage | Google Drive | Cloud storage with appropriate access controls |
| Notifications | Telegram | Email, Slack |
| Source access | Creator-authorized recording/feed/API | Platform-native clips or creator-provided files |
| Optional transcription | AssemblyAI | Whisper-compatible hosted service |

Tool availability, pricing, and API capabilities change. Verify current terms and capabilities before committing.

## Repository map

```text
ClipHunter-AI/
├── README.md
├── MASTER_PROMPT.md
├── PROJECT_STATUS.md
├── ROADMAP.md
├── CHANGELOG.md
├── .env.example
├── .gitignore
├── docs/
├── automation/make/
├── prompts/
├── data/
├── assets/
├── tests/
└── scripts/
```

## Quick start

1. Read [`MASTER_PROMPT.md`](MASTER_PROMPT.md).
2. Read [`docs/SECURITY_AND_PERMISSIONS.md`](docs/SECURITY_AND_PERMISSIONS.md).
3. Create a private GitHub repository named `ClipHunter-AI`.
4. Upload or push this folder to GitHub.
5. Copy `.env.example` to `.env` **only if using local code**; never commit `.env`.
6. Create Airtable base using [`docs/DATA_MODEL.md`](docs/DATA_MODEL.md).
7. Test the workflow using a short recording you own or have explicit permission to use.
8. Configure Make only after the manual process is understood.
9. Keep publishing disabled until the approval gate and rights checks pass.

## First MVP acceptance test

Given an authorized sample recording, the system should:
- register the source and permission reference;
- create one or more candidate highlights;
- produce a preview file or approved clipping-service output;
- store clip metadata and source timestamps;
- set each clip to `PENDING_REVIEW`;
- allow a reviewer to approve or reject;
- refuse to publish rejected or unreviewed clips;
- record an audit event for every decision.

## Important

This repository does not include credentials, API keys, creator agreements, or preconfigured live-stream access. Do not paste secrets into issues, chat, source files, or screenshots.
