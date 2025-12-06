# .ai-collab

My [AI Collaboration Profile](https://github.com/aself101/.ai-collab) — portable preferences for AI systems.

## What This Is

This repository contains my machine-readable collaboration preferences. Any ACP-compliant AI system can fetch and apply these to improve interaction quality.

## Files

| File | Purpose |
|------|---------|
| `profile.yaml` | Machine-readable preferences (required) |
| `guide.md` | Extended collaboration context (optional) |
| `projects/` | Project-specific overlays (optional) |

## Usage

AI systems can fetch my profile via:

\`\`\`
https://raw.githubusercontent.com/{username}/.ai-collab/main/profile.yaml
\`\`\`

Or with the [ai-collab](https://github.com/aself101/ai-collaboration-initiative) library:

\`\`\`javascript
import { fetchProfile } from 'ai-collab';
const profile = await fetchProfile('{username}');
\`\`\`

## Specification

See the [ACP Specification](https://github.com/aself101/ai-collaboration-initiative/blob/master/ai-collab-spec.md) for the full protocol definition.

## Privacy

See `profile.yaml` → `safety.visibility` for disclosure rules. Fields in `safety.avoid` should never be surfaced.
