# Phonics Adventure!

A browser-based phonics game for early readers (ages 4–7). Five mini-games cover spelling, sight words, rhyming, and beginning sounds — all in a single HTML file with zero dependencies.

## How to Play

Download or clone the repo and open `phonics-game.html` in any modern browser. No server, no install, no build step.

```bash
git clone https://github.com/thefalc/phonics-game.git
open phonics-game/phonics-game.html
```

## Mini-Games

### Word Builder
An emoji picture appears and the word is read aloud. Scrambled letter tiles are shown below — tap them in the correct order to spell the word. Covers CVC words (`cat`, `dog`), silent-e words (`joke`, `cake`, `kite`), vowel teams (`boat`, `rain`, `sight`), and blends (`truck`, `snake`, `globe`).

### Missing Sound
A word is shown with one letter replaced by a blank (e.g. `c _ k e`). Pick the correct letter from three choices. Mixes vowels and consonants across the full word bank.

### Sight Word Zap
Colorful bubbles float around the screen, each containing a sight word. A target word is displayed and spoken aloud — tap the matching bubble before it drifts away. Pulls from 60+ sight words including `the`, `because`, `would`, `their`, and `which`. 15 rounds per session.

### Rhyme Time
A word is shown with an emoji and read aloud. Pick which of three words rhymes with it. Covers 15 word families: `-at`, `-an`, `-ig`, `-op`, `-ug`, `-en`, `-it`, `-oke`, `-ight`, `-ake`, `-ine`, `-ope`, `-ide`, `-oat`, and `-ain`.

### Sound Spotter
An emoji picture appears (e.g. 🧀 for "cheese") and the word is spoken. Pick the beginning sound from three choices. Covers 14 blends and digraphs: `sh`, `ch`, `th`, `wh`, `bl`, `cl`, `fl`, `gl`, `br`, `cr`, `dr`, `fr`, `gr`, `tr`.

## Features

- **Text-to-speech** — Every word is spoken aloud using the Web Speech API. The game selects the most natural-sounding English voice available on the device, with separate tuning for clear word pronunciation and upbeat encouragement.
- **No penalties** — Wrong answers get a gentle nudge ("Almost!", "So close!") with no points lost. Encouragement only.
- **Varied feedback** — 16 unique cheers for correct answers plus streak bonuses ("Unstoppable!", "Turbo mode!") when you get 3+ right in a row. No two cheers repeat back-to-back.
- **Star rewards** — Every correct answer earns a star. Stars accumulate across all games and persist between browser sessions via `localStorage`.
- **Kid-friendly UI** — All buttons are at least 60px tall with large text, designed for small fingers on tablets and touchscreens.
- **Confetti animations** — Correct answers trigger a burst of colorful confetti. End-of-session summary shows animated stars.
- **80+ spelling words** — CVC, CVCe (silent-e), vowel teams, and blend words with emoji picture hints.

## Browser Support

Works in Chrome, Safari, Edge, and Firefox. Text-to-speech voice quality varies by browser and OS — Chrome and Safari on macOS tend to have the most natural voices.

## License

See [LICENSE](LICENSE) for details.
