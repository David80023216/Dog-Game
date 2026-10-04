# 🐾 Bark Avenue

A dog-themed mobile board game with Monopoly-Go-style mechanics — an **original game** (no Monopoly branding): roll the dice, buy pup properties, build dog houses up to Grand Kennels, and bankrupt your computer rival.

## Play it

🌍 **Play live now: https://bark-avenue-five.vercel.app/** (mobile portrait recommended)

Or open `index.html` in any modern browser, or deploy via GitHub Pages from this repo.

## Features

- 🎲 Dice roll with bet multiplier (1x / 2x / 5x / 10x)
- 🏘️ Dog-themed property color sets — buy, collect rent, build up to 5 levels
- 💰 Treat Heist vault mini-game & Shutdown events
- 🛡️ Chew Toy shields, 🃏 Lucky Leash chance cards, 🐶 Dog Pound (jail)
- 🖼️ "Pup Portraits" collectible album with set rewards
- 🗺️ Multiple boards — max out every landmark to advance
- 🏪 In-game shop (bones only, never real money)
- 🌍 Leaderboard — personal bests offline; global mode ready via `CONFIG.BACKEND_URL`
- 🤖 Solo vs computer AI opponent (Rex)
- 💾 Full game state saved in your browser (localStorage)

## Global leaderboard backend (optional)

Set `CONFIG.BACKEND_URL` at the top of `index.html` to a REST endpoint exposing:

- `GET {BACKEND_URL}/scores` → array of `{player, score, boards, date}`, top 20
- `POST {BACKEND_URL}/scores` with `{player, score, boards, date}`

When unset, the game runs fully offline with local personal bests.

Built with plain HTML/CSS/JS — zero dependencies, zero network requests.
