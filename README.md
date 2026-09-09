# Hot or Pot

A one-page trivia game: you get a name, and you decide whether it belongs to a
chili pepper (**Hot**), a cannabis strain (**Pot**), or **both**.

10 names per round, one point each, no repeats within a round. Play Again deals
a fresh random 10, which may include names you have seen before.

## Running it

Open `index.html` in a browser. That's it — no build step, no dependencies, no
network requests. It works from the filesystem or from any static host.

## Deploying to GitHub Pages

1. Push this repo to GitHub.
2. Settings → Pages → Source: **Deploy from a branch**, branch `main`, folder `/ (root)`.
3. The game appears at `https://<user>.github.io/<repo>/` after a minute or so.

## Editing the name list

The names live in the `RAW_NAMES` block near the top of the `<script>` in
`index.html`, one per line:

```
Ghost Train|Pot
Naga Viper|Hot
Mad Hatter|Both
```

Add or remove lines freely — the game reads whatever is there. `names.csv` in
this repo is the original source list, kept for reference; the game does not
read it at runtime.

To change the round length, edit `QUESTIONS_PER_ROUND` just below the list.
