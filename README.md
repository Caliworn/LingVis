# LingVis

Interactive, animated walkthroughs of ideas in linguistic theory — watch the derivations happen, step by step, node by node.

**Live site:** https://caliworn.github.io/LingVis/

## Visualizations

### Universal 20

[Open it →](https://caliworn.github.io/LingVis/universal20.html)

Of the 24 logically possible orders of demonstrative, numeral, adjective and noun, only 14 are attested. Following Cinque (2005), the page shows how one universal Merge order (Dem > Num > A > N), plus leftward movement of NP or of a phrase containing it, derives exactly those 14 — and why the other 10 cannot be derived.

- **Cyclic, bottom-up derivations.** Each tree is built by external Merge, one layer at a time, with Agr projections above each modifier. Movement is internal Merge into Spec,AgrP and is interleaved with Merge, never applied after the whole tree is built.
- **Every movement step is classified as in the paper:** NP movement without pied-piping, whose-picture pied-piping (including the vacuous case), picture-of-who pied-piping, re-raising of an already moved phrase, and the extraction step of N Dem A Num. Traces are left behind and co-indexed with what moved.
- **All 24 orders.** Each attested order shows its marked options and the frequency Cinque reports. Each unattested order is played out from the wrong Merge order it would require, with the offending modifier flagged.
- **Controls.** Autoplay; click the tree (or press →) to advance, and click during an animation to fast-forward it along the same path; ← to step back; Space to play or pause; R to restart; P to show movement paths.

## Running locally

Each page is a single, self-contained HTML file with no build step. Open `index.html` in a browser, or serve the folder so that the light/dark theme choice is shared between pages:

```bash
python -m http.server 8000
```

Then visit http://localhost:8000/.

## Project structure

```
index.html          landing page
universal20.html    Universal 20 visualization
```

## Source

Cinque, Guglielmo. 2005. Deriving Greenberg's Universal 20 and its exceptions. *Linguistic Inquiry* 36(3): 315–332.

The visualization paraphrases the paper's analysis; any errors in presenting it are the site's, not the paper's.

## Credits

Fonts: [Fraunces](https://fonts.google.com/specimen/Fraunces), [Inter](https://fonts.google.com/specimen/Inter) and [JetBrains Mono](https://fonts.google.com/specimen/JetBrains+Mono), via Google Fonts.

## License

[MIT](LICENSE) © 2026 Caliworn
