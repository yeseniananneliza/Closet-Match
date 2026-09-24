# Closet Match

Matches outfit formulas to what's already in your closet, based on your
body shape, undertone, and style preferences, then builds a shopping list
for what's missing.

**Live:** https://claude.ai/artifact/J3hUTxT1TDqGbA36ZyDfsd

Built as a scoped product case study, reusing the same core matching
mechanic as [Use It Up](https://github.com/yesenianannelicza/Use-It-Up):
what you have vs. what a formula needs, applied to a different domain.

## Stack
Single self-contained HTML file, vanilla JavaScript, no build step, no
framework. All 23 outfit formulas are embedded as JSON and matched
client-side.

## Run locally
Just open `index.html` in a browser, no server or install needed.

## Deliberate v1 scope decisions
- **Body shape and undertone are self-selected, not detected from a
  photo.** Skin-tone detection from images is a documented bias risk in
  computer vision, and collecting body photos is a real privacy liability.
- **No AI-generated "photo of you in this outfit" feature.** Realistic
  person-plus-garment image generation is a genuinely hard, compute-heavy
  ML problem on its own, and shipping it as a public, unauthenticated demo
  means anyone can upload a photo of anyone, that's the exact shape of
  feature that gets misused for non-consensual imagery of real people.
  Self-select and swatch-based matching get most of the user value without
  either the bias risk or that misuse surface.
- **Shopping links go to a general search, not a specific retailer's exact
  SKU.** No e-commerce API is wired up yet, so a search link is honest
  about what this actually is.

## What's scoped out of v1 (intentionally)
- Photo-based body/skin detection or AI outfit-on-you image generation
- Real e-commerce API for exact, in-stock product links
- Saved/persistent closets across visits
- User accounts

These are the natural v2 roadmap, cut from v1 to validate the core loop
fast, not gaps that were missed.
