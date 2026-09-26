# Contributing to Leave Discord

Thanks for considering a contribution. This project is a single static HTML page, so most changes are simple text or data edits.

## Ways to help

- **Fix outdated information** — a service changed its pricing, platforms, or encryption model, a link is dead, or a leak/incident needs correcting.
- **Add a new alternative** — propose a service that fits the same criteria (a real Discord alternative: chat, voice, and/or video for communities).
- **Improve a translation** — the English and French versions should stay equivalent in meaning; point out anything that drifted.
- **Accessibility and design** — color contrast, keyboard navigation, screen-reader labels, responsive layout.
- **Bugs** — anything that doesn't behave as expected (the quiz, the filters, the comparison table, the language switch).

## Before you open a pull request

1. **Check your facts.** For data changes (leak counts, trust ratings, dates, pricing, platform support), link to a source in your pull request description — ideally the service's own site, a press release, or reputable reporting.
2. **Keep entries balanced.** Each alternative's card lists at least one honest limitation alongside its strengths. Please don't turn a listing into pure marketing copy, for or against any service.
3. **Update both languages.** If you change English copy that has a French equivalent (or vice versa), update both, or flag in your PR that a translation update is still needed.
4. **Test in a browser.** Since this is a single HTML file with no build step, just open it directly and click through all three pages (Home, Compare, Find your alternative) in both languages before submitting.

## Adding a new alternative

Each service is one entry in the `S` (or `S_EN` / `S_FR`) data array near the bottom of the file, with a matching row in the comparison table and, optionally, weighting in the quiz's `Q` array. An entry needs:

- `id` — a short unique code (2–3 letters)
- `n` — display name
- `k` — a short one-line description
- `c` — founding year
- `lk` / `lt` — number of known major leaks, and a short description (omit `lt` if `lk` is 0)
- `t` — trust rating, 1 (low) to 5 (very high), with a one-line editorial justification you can defend if asked
- `p` — platform codes (`A` iOS/macOS, `a` Android, `W` Windows, `x` Linux, `w` Web)
- `pr` — price line
- `tb` — `[end-to-end encryption, voice, video, open source, free]`, each `0` (no), `1` (yes), or `2` (partial)
- `x` — space-separated filter tags (`e2e`, `self`, `noid`)
- `u`, `d`, `pro`, `con` — official URL, one-paragraph description, one strength, one limitation

## Reporting an issue

Open an issue describing what's wrong and, where relevant, a source or a screenshot. There's no formal template — clarity matters more than format.

## Code of conduct

Be respectful and assume good faith. Disagreements about which service deserves a higher trust rating are expected — resolve them with sources, not volume.
