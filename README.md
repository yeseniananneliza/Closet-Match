# Closet Match

Outfit ideas matched to your body shape, undertone and style, built from the clothes you already own.

**Live site:** https://yeseniananneliza.github.io/Closet-Match/?v=2

## What it does
- Pick your body shape, undertone and favorite styles to get a personalized "For you" board
- Tap the pieces you own, and every outfit shows what you already have
- Browse all 23 outfit ideas in Explore, or search by piece, color or occasion
- Save outfits to build one combined shopping list of the pieces you're missing, with a link to shop each one
- Your closet and saved outfits are remembered in your browser

## Built with
A single HTML file with plain CSS and JavaScript. No framework, no build step and no backend. Open `index.html` in a browser to run it locally.

## Product decisions
- **Body shape and undertone are self-selected, not detected from a photo.** Skin-tone detection from images is a documented bias risk, and collecting body photos is a privacy liability.
- **No AI "see yourself in this outfit" feature.** Realistic images of a real person are hard to generate well, and on a public site anyone could upload a photo of anyone.
- **Shopping links open a search, not a specific retailer's product.** There's no store integration yet, so a search is honest about what the link does.

## What's next
A larger stylist-reviewed outfit set, a "one piece away" view that ranks purchases by how many new outfits they unlock, and accounts so a closet follows you between devices.
