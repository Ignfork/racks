# Racks ($RACKS)

One coin, one pool and 100 server racks in a pixel datacenter warehouse with a 2000s internet look. The pool's liquidity is cut into 100 price bands, and each rack owns one band. The rack the price is sitting in earns every swap fee in that band.

## Deploy
The site is a single `index.html` with no folders and no build step. Drop it into a GitHub repo or Vercel.

## Settings
Open `index.html` and find `CONFIG` near the top of the script:

```js
var CONFIG={xUrl:'',ca:'',buyUrl:'',chartUrl:''};
```

To rename the project, search and replace `Racks`, `RACKS` and `racks`.

## What's on the page
- **Warehouse hero:** a NOC wall of 18 monitors, rows of racks with blinking lights, a night-shift desk with CRTs, a forklift, a tape cart and boxes. The running rack glows, and racks flash when a bit flip lands. Parts of the room are clickable.
- **Floor map:** a 10×10 grid of racks (RK-00 to RK-99) with filters for all, unminted, listed and yours, plus liquidity bars for every band.
- **Pool stats:** price, band in range, fee now, jobs, flips, minted, SOL earned and locked, and the last job hash.
- **Inspector:** the rack's art, its 8-byte spec (clock, ecc, bus, cache, s0 to s3), fee, status, band, liquidity, earnings, and mint and track buttons.
- **Logs:** a live jobs log and a bit flips log (landed flip or ECC caught).
- **Info:** a readme, FAQ and the $RACKS token section.

Contracts are not connected yet, so all prices, jobs, flips and balances are a labelled simulation.
