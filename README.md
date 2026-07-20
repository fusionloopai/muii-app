# Metoxi

**Decision Space by FusionLoop AI** — an app that coaches you through making better decisions, then tracks whether they worked.

Built on Tony Robbins' OCEMR process plus Josh Holladay's additions. The flow:

1. **Name It** — what's the decision?
2. **Outcomes** — what do you want? (experiences, things, people, what you create for others)
3. **Reasons** — why do you want each one? The why is the fuel.
4. **Order** — drag-rank what matters most *for this season of your life*. "Later" outcomes stay on the Target list so the future never gets lost.
5. **Options** — one option is no option, two is a dilemma. Three to be a choice.
6. **Consequences** — upsides and downsides of each option.
7. **Evaluate** — probability × impact sliders on every consequence. Live score per option.
8. **Mitigate** — shrink the biggest risks, mix and match options into hybrids.
9. **Resolve** — choose, commit, one action today, review date. Then track results.

The dashboard has four lenses: **Track** (decisions + results), **Target** (short-term and long-term outcome lists), **Trim** (paths you chose not to take — on the record so they stop haunting you), **Train** (your decision-making stats).

## Running it

It's one file. Open `index.html` in any browser, or serve it:

```bash
python3 -m http.server 4820
# → http://localhost:4820
```

## Your data

Everything lives in your browser's localStorage — nothing leaves your machine. Use **Export** to download a JSON backup, **Import** to restore it (or move to another browser/device).

## Stack

Single-file vanilla JS SPA, no build step, no dependencies beyond two CDN loads (Google Fonts, Phosphor Icons). Theme matches rofa.fusionloop.io. v2 direction: Zentile-style hosted backend (Supabase/PostgREST) for sync and multi-device.
