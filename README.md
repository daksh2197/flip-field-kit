# Flip Field Kit

**Know your walk-away price before the auctioneer or the yard does.**

One page, two modes, no sign-up:

- **Auction max bid.** Type the sold prices you found (the kit takes the median, so one lucky sale doesn't set your price), the buyer's premium, GST, haul and repair costs, the selling platform's fee, and the profit you want. It gives you the hammer price to stop at and the all-in cost at the till.
- **Pick-and-pull parts.** List the parts you plan to pull with the yard price, what each sells for and the shipping. Each part gets a Pull, Thin or Skip call against your minimum profit, plus a link to eBay sold listings for that part.
- **Flip log.** Save a lot or a yard trip, then fill in what you paid and what it sold for. The log shows your real profit. It stays in your browser (localStorage), and nothing is sent anywhere.

## The maths

```
walk-away bid = (resale × (1 − fee%) − fixed fee − shipping − haul − repairs − target profit − hours × $/hour)
                ÷ ((1 + buyer's premium%) × (1 + GST))
```

GST is 5% in Alberta, which has no provincial sales tax. Untick it where it doesn't apply, or where you're registered to claim it back.

## What it won't do

- **Guess fees.** Buyer's premiums, platform fees and yard prices change by auction, platform and yard. Type the current ones. The example buttons are labelled as examples.
- **Scrape listing sites.** The comp links open eBay sold listings, Facebook Marketplace Calgary, Kijiji Calgary and GCSurplus in a new tab. Pulling sold prices in automatically is next, through the eBay Browse API.

## Run it

It's one HTML file. Open `index.html` in a browser, or turn on GitHub Pages for this repo (Settings → Pages → Deploy from branch → `main`, root).

## What's next

- [ ] eBay Browse API sold-price lookup (free developer key, kept on your device)
- [ ] Export the flip log to CSV
- [ ] Saved fee presets per auction house and platform

## License

MIT
