# Surfside Timer

A tiny, local web app for running several stopwatches side by side — one per language — so a bilingual meeting can keep each language's speaking time honest.

Open one HTML file. No install, no build, no internet required.

## Why

We run meetings where speaking time is shared between two languages. When the conversation switches languages, you pause one timer and start the other.

The catch: sometimes a speaker translates for themselves, which quietly spends time on both sides at once. With a single shared clock there's no way to see that happening. Surfside Timer gives each language its own countdown, so everyone can glance up and see exactly how much of their parallel 3 minutes (or whatever you set) each side has left. Nobody has to keep it in their head.

## Using it

1. Open `index.html` in any modern browser (double-click it, or [try the live version](https://surfside-pr.github.io/multilingual-countdown-timer/)).
2. Set the duration up top (defaults to **3:00**). Every track shares it.
3. Hit **play** on a track to start its countdown — only one runs at a time.
4. When the conversation switches, press **Space** to pause the current track and hand the clock to the next one.

That's the whole loop. Tracks default to **Spanish** and **English**; rename them, recolor them, or add more with **+ Add language**.

When a track hits 0:00 it doesn't stop — it rolls into overtime and starts a gentle pink-to-red flash, so it's obvious which side has run over without anyone needing to say so.

## Keyboard shortcuts

| Key | Action |
| --- | --- |
| `Space` | Pause the active track and advance to the next one (wraps around) |
| `P` | Pause / resume the active track without advancing — handy for a quick aside |
| `R` | Reset all tracks to the duration |
| `Enter` | Commit an edit (duration, label, or a track's time) |
| `Esc` | Cancel an edit / close a menu |

You can also click any track's time to edit it directly, and each track's `…` menu has color, per-track reset, and remove.

## Built with

Plain HTML, CSS, and JavaScript — no frameworks, no dependencies, all inlined into a single `index.html`. The whole app is the one file you open.
