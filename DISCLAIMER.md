# Disclaimer

The contents of this repository are provided **for informational and research
purposes only**. They are **not financial, investment, or trading advice**, and
nothing here should be construed as a recommendation to buy, sell, or hold any
trading card, collectible, or other asset.

## What this is

- A composite index that estimates how wanted a Magic: The Gathering card is
  right now (buy-side desire to acquire it), based on public data: Commander
  popularity (EDHREC inclusion), sustained price appreciation, format
  playability, and how widely the card has been printed.
- The model produces a relative score from 0 to 100, not a guarantee. A high
  score means the card currently behaves like other cards that are heavily
  wanted; it does not promise future price movement or continued demand.

## What this is not

- It is **not** a forecast of future card prices.
- It is **not** the same as liquidity (how easily a card can be sold). Demand is
  how much the market wants to buy; liquidity is how easily an owner can exit.
- It is **not** a measure of what a card is worth.
- It is **not** a substitute for your own judgment or for professional advice.
- It does **not** account for your individual financial situation, collection,
  tax position, or risk tolerance.

## Honest limitations

- This is version 1, a transparent composite index, not a supervised forecast.
  There is no single clean ground-truth label for "demand", so it carries no
  held-out accuracy score. It is validated by internal consistency and by
  independent corroboration instead.
- It measures demand **level**, not demand **growth**. It uses a current EDHREC
  snapshot, not an EDHREC time-series, so it cannot yet tell a card climbing in
  popularity from one fading at the same level.
- EDHREC popularity is a Commander-format signal. It is the best direct demand
  measurement available for the secondary market, but it under-weights demand
  that lives mostly in competitive constructed formats.
- A Commander ban shows up as lost demand once (EDHREC drops banned cards).
  Cards banned only in competitive formats carry no penalty, because being
  banned for power is not the same as low demand.

## No warranty

Outputs in this repository are provided "as is", without warranty of any
kind, express or implied, including but not limited to warranties of
merchantability, fitness for a particular purpose, accuracy, or
non-infringement. **The authors accept no liability** for losses, missed
gains, or any other damages arising from use of this material.

Cards and game terminology are property of Wizards of the Coast LLC. This
project is not affiliated with, endorsed by, or sponsored by Wizards of the
Coast.

By Cameraderie Cards.
