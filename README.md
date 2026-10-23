# Scrap to Scale

A browser game that teaches circular economy principles. You run a company in a shared economy where one firm's waste is another firm's raw material. Build partnerships, recover products after use, and keep materials circulating while staying profitable.

No build step, no dependencies. Open `index.html` in a browser.

## Built for beginners

- Four short lessons explain linear vs circular economy before play begins.
- Every technical word (dotted underline) can be tapped for a plain-language definition, and a Glossary button lists all terms.
- A mentor suggests a good move at each step and pre-sets the sliders.
- After each step, a "What happened" summary and a "Key idea" connect the result to the concept.
- The final report explains the score and what to try next.

To add or edit vocabulary, change the `G` object in `index.html`. Write `[[key|shown text]]` in any text to make it a tappable term.

## Play

Choose a business: clothing maker, furniture maker, food producer, or construction firm. You get 10 rounds. Each round follows the core loop:

| Step | What you do | Concept it teaches |
|---|---|---|
| Source | Buy virgin material or reclaimed byproducts from another firm | Input substitution, price risk, material quality |
| Produce and sell | Choose output and price against customer demand | Production creates waste and products that will become waste |
| Recover | Repair, recycle, or dump products that customers return | Value retention hierarchy: repair > recycle > dispose |
| Trade | Sell your production waste to a partner firm | Industrial symbiosis, transport costs, repeat partnerships |
| Improve | Invest in collection, repair, waste-saving design, sorting | Reinvesting profit into circular capability |

Random events (virgin shortages, landfill taxes, green customers) show why circular models are more resilient.

## Scoring

- **Profit**: final cash minus starting cash.
- **Loop outflow %**: share of waste and returned products that were traded, repaired, or recycled instead of dumped.
- **Loop inflow %**: share of material you used that came from reclaimed sources.

A run counts as a circular business when it is profitable and keeps at least 60% of outflows in the loop.

## Publish on GitHub Pages

1. Push this folder to a repository.
2. Go to Settings → Pages, choose the `main` branch and the root folder.
3. Your game will be live at `https://<username>.github.io/<repo>/`.

## Customise

- Businesses, prices, and partners: the `BIZ` object in `index.html`.
- Random events: the `EVENTS` array.
- Upgrades: the `UPG` array and `RATE` (collection rates).
- Length: the `ROUNDS` constant.

## Ideas for next steps

- Hot-seat or online multiplayer where each player's waste is actually another player's input.
- Add the other actors from the design: repair shops, collectors, and customers as separate agents.
- Chart of loop % per round, and a "linear company" baseline for comparison.
- Quality grades for byproducts and negotiated prices.

## License

MIT. Add a `LICENSE` file when you publish.
