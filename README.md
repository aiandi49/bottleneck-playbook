# Compass — A Hub of Real Business Playbooks

Most owners already know the theory. What trips people up is the order of operations — what to fix first, what to leave alone, and what to never touch until the earlier steps are done.

Compass turns real, recorded business turnarounds into playbooks you can actually follow, step by step. Each guide breaks a real conversation down into a numbered sequence, with plain-English explanations, key-term callouts, a "do this" checklist that saves your progress, and the actual before/after results.

## Structure

This repo is a static site — no build step, no dependencies. Open any `.html` file directly in a browser, or serve the folder with GitHub Pages.

| File | What it is |
|---|---|
| `index.html` | The Compass hub home — a "start here" triage, foundational start-a-business guidance, and the playbook library |
| `bottleneck-playbook.html` | Playbook 1: scaling a business that's capped by a single bottleneck |
| `cash-flow-rescue.html` | Playbook 2: rescuing a business that's close to running out of cash |
| `menu-close-playbook.html` | Playbook 3: raising revenue per job in a service business through offer, close, and channel focus |
| `referral-machine-playbook.html` | Playbook 4: engineering referrals and trust for high-ticket sales — includes an honest "plan met reality" pivot instead of a clean win |
| `field-notes.html` | Founder Field Notes — a non-sequential reference of standalone ideas on starting, pricing, hiring, growth, and mindset |

`index.html` is the entry point (this is what GitHub Pages will serve at the repo's root URL). Each playbook links back to it via the breadcrumb bar in its header.

## Adding a new playbook

1. Duplicate `cash-flow-rescue.html` as a starting template.
2. Swap in the new case study's content — hero, context cards, numbered chapters, results, pitfalls.
3. Give its checklist a unique storage key (search for `-progress` in the `<script>` block) so its saved checkboxes don't collide with other playbooks.
4. Add a card for it in the `#library` section of `index.html`, and point its breadcrumb bar back to `index.html`.

## Adding to Founder Field Notes

`field-notes.html` is reference material, not a sequence — no checklist, no progress tracking. To add a new note, drop a `.note-card` into the relevant `.note-grid` (or add a new `.note-section` for a new topic and link it from the quick-nav at the top). Cross-link from a playbook from a specific move using an anchor, e.g. `field-notes.html#pricing`.

## Notes

- All pages are fully self-contained (inline CSS/JS) — no shared stylesheet, so each page also works fine if opened on its own.
- Checklist progress is saved per-device using the browser's artifact storage, keyed per playbook.
- Educational content only. Every business is different — treat these as starting sequences to test against your own numbers, not a guarantee of results. Not affiliated with, endorsed by, or produced by Alex Hormozi or Acquisition.com.
