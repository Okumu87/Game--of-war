# Game of War

Simple browser implementation of the classic card game "War".

## Project overview
- **Purpose:** Lightweight game demo using the Deck of Cards API for shuffling and drawing cards.
- **Files:** index.html, script.js, style.css

## Features
- Start a new shuffled deck (via script.js).
- Draw cards and compare values to determine round winners.

## How to run
1. Open index.html in your browser (no build step required).
2. Click the "New Deck" / game buttons provided in the UI to interact.

## API
- Uses the Deck of Cards API (https://deckofcardsapi.com/). `script.js` fetches a shuffled deck from the API.

## Development notes
- Entry point: index.html (UI). Main logic in script.js.
- Example snippet used to initialize a deck (from script.js):

```js
fetch("https://apis.scrimba.com/deckofcards/api/deck/new/shuffle/")
  .then(res => res.json())
  .then(data => {
    console.log(data)
    deckId = data.deck_id
  })
```

## Contributing / Updates
- I can help update and expand this README regularly (features, screenshots, gameplay rules, tests).
- To request updates, tell me what to add (badges, deployment, screenshots, usage examples, or a changelog).

## License
Add your preferred license here (e.g., MIT).
