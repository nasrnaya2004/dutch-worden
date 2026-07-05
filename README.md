# Dutch Woorden

A personal flashcard app for learning Dutch vocabulary and verb conjugations, built as an installable web app (PWA).
https://nasrnaya2004.github.io/dutch-worden/

## Features

- **Flashcard practice** — study words by category or shuffle everything together, with configurable direction (English → Dutch or Dutch → English)
- **Verb conjugation drills** — practice conjugating verbs across pronouns, with instant right/wrong feedback
- **Word list view** — browse all saved words and categories at a glance
- **Excel-based vocabulary import** — upload an `.xlsx` file to add/update words; the app parses it client-side and syncs to GitHub automatically
- **Cross-device sync** — vocabulary data is stored in `words.json` in this repo, so progress and word lists are the same on every device
- **Installable** — works as a home-screen app on iOS/Android with offline-capable manifest and service worker

## How it works

1. Open **Settings** and add a GitHub personal access token (used only to save/update `words.json` in this repo — see in-app instructions for generating one)
2. Upload an `.xlsx` file with two columns: English (A) and Dutch (B), with category headers as merged cells
3. A second sheet can hold verb conjugations (verb name + pronoun/form pairs) for the Conjugate tab
4. Words and verbs sync to GitHub and load automatically on any device

## Excel format

| Column A | Column B |
|---|---|
| *Category title (merged row)* | |
| hello | hallo |
| goodbye | tot ziens |
| *Food (merged row)* | |
| to eat | eten |

## Tech

Single-file HTML/CSS/JS app — no build step, no dependencies. Includes a minimal in-browser `.xlsx` parser (unzips and reads the OOXML directly) so no external libraries are needed.
