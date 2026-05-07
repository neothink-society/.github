# Neothink

Engineering home for the body of work originated by Mark Hamilton across fifty years of independent research. This GitHub org hosts the source for the public sites, the member-facing platform, and the supporting infrastructure. All source repositories are private.

## Entities

| Domain | Entity | What it is |
| --- | --- | --- |
| [neothink.com](https://www.neothink.com) | Neothink Institute | An independent research institution. Restoring man to his nature and building the civilization that comes after. |
| [neothinksociety.com](https://www.neothinksociety.com) | The Neothink Society | A private worldwide society where members use the Neothink mind in business, relationships, health, prosperity, productivity, self-leadership, and the pursuit of abiding happiness. Operating across 140 countries for decades. |
| [joinneovia.com](https://www.joinneovia.com) | Neovia | The civilization that was always possible. The first civilization designed from the ground up to remove hierarchy and initiated force as governing principles. |
| [markhamilton.co](https://markhamilton.co) | Mark Hamilton | American civilizational theorist and institutional founder. Architect of the Unified Field of Conscious Civilization and originator of Neovia. Five decades of independent research. |
| [wallacehamilton.co](https://wallacehamilton.co) | Wallace Hamilton | Voice of The Way. Co-host of Unleashed. |

The Institute publishes the body of work. The Society is one place where the work becomes practice. Mark Hamilton originated the framework. Wallace Hamilton voices The Way. Each entity runs as a distinct surface and is referenced under its own name.

## Marketing surfaces

| Domain | Origin | What it is |
| --- | --- | --- |
| [theway.world](https://theway.world) | Wallace Hamilton | The Way. The personal path of removing falsehood and restoring direct sight. The individual expression of the Unified Field. |
| [aristotlepower.com](https://aristotlepower.com) | Mark Hamilton | The Aristotelian Thinking. Live class registration. |
| [masterclass.wallacehamilton.co](https://masterclass.wallacehamilton.co) | Wallace Hamilton | Live webinar funnel. |

## Platform

A Turborepo monorepo powers the member-facing experience.

### Apps

| App | Domain | Purpose |
| --- | --- | --- |
| `admin` | `admin.neothink.io` | Internal operations dashboard. AI chat, workflows, content ops. |
| `web` | `app.neothink.io` | Member journey portal. Levels 1 through 4, workbooks, progress. |
| `community` | `network.neothink.io` | Social platform. Feed, discussions, events, courses. |
| `invitation` | `invitation.neothink.io` | Live webinar surface (Zoom Video SDK). |
| `mobile` | (Expo) | React Native member app. In development. |

### Shared packages

`@neothink/supabase` (auto-generated DB types and client helpers), `@neothink/ai` (AI SDK v6 wrapper through the Vercel AI Gateway), `@neothink/design-system` (Tailwind v4 tokens and Liquid Glass materials), `@neothink/email` (React Email plus Resend), `@neothink/utils` (validation and formatting), `@neothink/ghl` (GoHighLevel read helpers).

### Agents

`agents/neosis` is a LiveKit Agents voice AI written in Python and deployed on LiveKit Cloud.

## Stack

- **Web:** Next.js 16, React 19, TypeScript 6, Tailwind CSS v4, shadcn/ui, Turborepo, Turbopack, pnpm.
- **Database and auth:** Supabase. Postgres, Auth, Realtime, Storage, Edge Functions, pgvector.
- **AI:** Vercel AI SDK v6 through the AI Gateway. Default model is Gemini 2.5 Flash-Lite. AI Elements and Streamdown for chat UI.
- **Infrastructure:** Vercel Fluid Compute. Workflow SDK for durable jobs. Skip-unaffected deploys via affected-projects detection.
- **Email:** Resend plus React Email.
- **Voice and video:** LiveKit Agents (Python). Zoom Video SDK (web and React Native).
- **Mobile:** Expo, React Native, React Native Reusables, NativeWind.
- **CRM:** GoHighLevel as legacy reporting integration. Supabase is the source of truth for all member data.

## Voice and brand quick reference

For anyone writing copy, commit messages, or UI strings that touch a public surface:

- **Speak from reality.** Describe truth so the reader recognizes it, rather than making claims the reader has to evaluate.
- **Define entities by what they are.** Do not reach for negative classifications to deny.
- **Each entity owns its own voice.** The Institute speaks in institutional-claim mode. The Society speaks in applied-practice mode. The Way speaks in subtractive recognition. Neovia speaks in architectural mode. Mark Hamilton speaks in person mode. Vocabulary does not cross between entities.
- **No em dashes or en dashes** in user-facing copy. Use periods, semicolons, colons, or restructure.
- **No "not X, but Y" comma constructions.** Break with periods.
- **Canonical lines repeat verbatim.** Do not paraphrase canonical lines by accident.
- **Neothink** is one word, capital N. Never `Neo-Think` or `NeoThink`.
- **Neo-Tech** is hyphenated.
- **Mark Hamilton** carries no middle initial. **Frank R. Wallace** is referenced with the R.

Full brand and voice guidance is maintained outside this repo and held privately.

## Contact

General: [admin@neothink.io](mailto:admin@neothink.io)
