# nextunit-kit feedback

Public issue tracker for [nextunit-kit](https://github.com/nextunit-io/ai-development-kit), a Claude Code plugin marketplace for AI-assisted development.

Anyone can open an issue here. Most issues are written by the kit itself: after a retrospective or a sync, `/nextunit-kit:feedback` offers findings about the kit, and the user decides which ones to send.

## What an issue contains

- The kit component: an agent, gate, script, skill or `AGENTS.md` region of the kit.
- A category: `instruction-misled`, `noisy-gate`, `missing-check`, `script-error`, `escalation`, `upstream-candidate` or `docs`.
- A short topic, what happened, what was expected, and a suggestion (each at most 300 characters).
- Numbers only as evidence: rounds, escalations, QA loops, dismissed issues, items.
- The kit version, the language packs, the phase, and a fingerprint `component:category:topic`.

## What an issue never contains

Code, file paths, URLs, email addresses, item IDs, review comments, or the name of the project or its owner. The kit script removes these before the user sees the text, and the user sees the exact text before anything is sent.

## How fixes are confirmed

1. The same problem always gets the same fingerprint, so reports from different repositories land on one issue as comments.
2. A release that fixes an issue says `Fixes feedback#<n>` in its CHANGELOG.
3. After a target updates, the kit watches for the fingerprint again. If the problem comes back, it offers a "recurred" comment. If it stays away for five merged items, it offers a "confirmed fixed" comment.

## Labels

- `kit-feedback`: every issue from the issue form or the kit.
