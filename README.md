# OKX copy trading: what does it cost, why do some orders never copy, and how should you read Win rate and PnL%? (settings checklist included)

OKX copy trading on the spot market runs with no leverage and no liquidation risk, charges the same trading fee as a manual spot order, and pays the lead trader you copy up to 30% of profits. The spot product went live globally in November 2023, quotes every lead trade in USDT, and supports 114 cryptocurrencies as the base currency.

Below is what the fee actually deducts and when, the 0.5% price rule that silently cancels copies, how the five numbers on a lead trader's profile are calculated, and which settings to fill in before you risk anything.

> **Quick verdict:** start with Spot copy trading rather than futures. There is no liquidation, so your worst case is the coin falling, not a forced close. Fill in **Maximum total amount** and **Stop loss for trader** before your first copy, then run a small fixed-amount copy for a week to see how many of the lead trader's orders actually land in your account.
> 👉 [Open the OKX copy trading sign-up entry](https://okx.com/join/CASH20)

## Four product lines sit behind the same button, and none of them is a subscription

OKX does not sell copy trading as a monthly plan. There is no Starter tier, no Pro tier, no subscription fee and no per-seat pricing. What people call "plans" on other comparison pages is either the product line you pick or the profit-sharing ratio the lead trader sets.

On web you reach everything through **Trade > Bots & Copy > Copy trading**, then switch between Futures copy trading, Spot copy trading, Bot marketplace and Signal marketplace. In the app it is **Trade** (tap twice) **> Bots & Copy > Recommended**, scroll to Copy trading, and switch between Futures / Spot / Bots / Signal.

| Product line | What it is | Leverage | How you pay | Suits |
| --- | --- | --- | --- | --- |
| Spot copy trading | Your account automatically repeats a lead trader's spot buy and sell orders | None, no liquidation | Standard spot trading fee + up to 30% profit share to the lead trader | First-time copiers, people who want to hold coins without a margin call |
| Futures copy trading | Mirrors a lead trader's perpetual futures positions, with contract, margin mode and leverage settings | Yes, you set it per contract | Trading fee + profit share; funding payments apply | People who already trade futures and can manage a forced close |
| Bot marketplace | Copies or subscribes to automated grid/DCA style bots | Depends on the bot | Per the bot's own rules | Hands-off strategies where you are not following a person |
| Signal marketplace | Follows published trade signals rather than an account | Depends on how you execute the signal | Per the signal provider | Traders who want ideas but place orders themselves |

👉 [Start on the spot copy trading entry](https://okx.com/join/CASH20)

## What you actually pay: a normal spot fee plus up to 30% of profits

Two costs exist, and they are charged at different moments.

**The trading fee** is identical to a manual spot trade. OKX does not add a copy-trading surcharge. Your exact maker/taker rate depends on your own fee tier and is displayed on the order confirmation, so the number you should check is your own, not a generic rate from a blog.

**The profit share** goes to the lead trader. Lead traders set their ratio according to their trader level, with a maximum cap of 30%, and the ratio is shown on the copy trading page for the trader you are considering. Read it before you copy. A trader charging 10% and a trader charging 30% produce very different net results from the same gross profit.

### How the weekly settlement works

The settlement cycle runs **every Monday 00:00 (UTC+8) to Sunday 23:59:59 (UTC+8)**, and profit sharing is calculated every Monday at 00:00 (UTC+8).

When a copied position closes at a profit, the system deducts the trading fee first, then withholds the profit-share amount on that trade. On the settlement day it calculates your total PnL across the whole week and pays the lead trader the real amount owed. Any excess withheld during the week is returned to your trading account.

That refund matters because individual winning trades can over-withhold when the week nets lower. The official example uses a lead trader at level L2 charging 10%:

| Date | Trade | PnL after fees | Withheld (10%) |
| --- | --- | --- | --- |
| Apr 17 | BTC/USDT sold | +200 USDT | 20 USDT |
| Apr 18 | BTC/USDT sold | −50 USDT | 0 |
| Apr 18 | ETH/USDT sold | +300 USDT | 30 USDT |
| Apr 20 | ETC/USDT sold | −500 USDT | 0 |
| Apr 22 | ETC/USDT sold | +500 USDT | 50 USDT |
| Apr 23 | BTC/USDT sold | +100 USDT | 10 USDT |

Net PnL for the week is 550 USDT. Total withheld is 110 USDT. The lead trader is actually owed 550 × 10% = 55 USDT, so 55 USDT comes back to the copy trader. Had you judged the cost from the individual winning trades alone, you would have overestimated it by half.

### The clause that delays your settlement

Profit sharing is only settled when you are not copying any ongoing trades from that lead trader. If you still hold an open copied position, settlement is pushed to the first settlement date on which you have no ongoing spot copies.

This is the part almost no guide mentions. A copy trader who keeps a permanent position open can go weeks without a settlement, with withheld amounts sitting unresolved. If you care about clean accounting, plan to close out copied positions before a Monday.

You can find the actual transactions under **Trading > Transactions > Transaction types > Other**.

## Why your position doesn't match the lead trader's: the 0.5% rule and four other conditions

A copy order is placed only when five things are true at the same time:

1. The coin supports spot copy trading.
2. Your trading account holds enough USDT for the order.
3. The order value is above the minimum limit for that coin.
4. The gap between the lead trader's buy price and your buy price is **no more than 0.5%**.
5. The lead trader has not triggered risk control.

Condition four is the one that quietly changes your results. The lead trader fills, the price moves, and by the time your order would execute the difference is above 0.5%, so no buy order is placed at all. You end up with a portfolio that looks like the lead trader's but is missing the entries that ran away fastest. Sells work differently: when the lead trader sells, a sell order is placed for you, and your execution price may differ slightly from theirs.

Two more mechanics to know:

- **Bought coins are frozen.** Anything you buy through a spot copy trade cannot be used for other purposes until you sell it. Frozen assets are visible under your assets.
- **Minimum purchase amounts vary by coin** and shift with price. Check the asset details on the manual trading page rather than assuming a fixed USDT floor. (The 10 USDT minimum people quote belongs to the futures side, covered below.)

You are not locked in until the lead trader exits. You can manually sell copied assets before they do, from the Copy Trading management page, and your PnL is calculated from your own buy and sell prices.

👉 [Set up a small first copy on OKX](https://okx.com/join/CASH20)

## Reading the five numbers on a lead trader's profile

Profiles refresh hourly and show five metrics. Two of them are routinely misread.

| Metric | Official definition | How to read it |
| --- | --- | --- |
| AUM | Total investment of all copy traders; each copy trader counts at the smaller of their max total copy amount or their trading account USDT equity | Measures how much money follows this trader, not how good they are |
| PnL | Total profit or loss from this trader's spot lead trades | Absolute number, so a large account will always look impressive |
| PnL% | PnL ÷ maximum investment during the selected period; the calculation includes funds transferred in and out | Always check which period is selected before comparing two traders |
| Lead trader investment | USDT in the lead trader's own trading account | The best proxy for whether they have skin in the game |
| Win rate | **Number of days with profitable trades ÷ number of days the trader has led spot trades** | A daily measure, not a per-trade hit rate |

The win rate definition is the trap. A trader showing 70% is profitable on 7 days out of 10, not on 7 trades out of 10. Someone with a 60% daily win rate can still lose money on most individual trades if the losing days are heavy. Treat it as consistency, not accuracy.

PnL% has a second trap. Because the denominator includes deposits and withdrawals during the period, it is not an annualized return and cannot be lined up against a fund's published performance.

A workable screening order: first look at **Lead trader investment** and check whether their own capital is anywhere near the size you plan to commit. A trader running a few hundred USDT and a trader running six figures behave differently when sizing orders. Then check the period setting behind PnL%, and only then compare win rates between shortlisted traders.

## The settings that decide your risk

Spot copy trading asks for the following when you set up a copy:

- **Copy trade amount type.** Fixed amount invests the same USDT value in every copied order. Proportional amount multiplies the lead trader's order value by your multiplier: if they order 1,000 USDT at 0.1x, you order 100 USDT.
- **Amount per copy.** The fixed USDT figure or the multiplier itself.
- **Maximum total amount.** The ceiling on everything you invest under that one lead trader. Once reached, new buy orders stop being copied until you sell the spot you are holding. This is your real exposure limit, and it is the field most people leave blank.
- **Copy trade crypto.** Restricts copying to one coin. Keeping it aligned with the lead trader's own pair is the safer default.
- **Stop loss for trader.** The maximum total loss you accept across all trades under that lead trader. When cumulative losses hit it, copying stops, and any unsold assets are handled according to the action you set.
- **Take profit per order / Stop loss per order.** Per-order exits rather than account-level ones.

### Futures-only settings, kept separate

These apply to futures copy trading and not to spot:

- **Minimum 10 USDT** in the Amount per order field.
- **Contract settings:** same as trader or a custom contract list, with cross, isolated or same-as-trader margin mode.
- **Leverage**, which OKX recommends keeping **below 20x**.
- When your maximum copy total is reached, the system stops opening new positions until existing ones close.

Mixing these into a spot setup is a common mistake. Spot copy trades have no leverage field at all, and no liquidation price to watch.

## Smart Sync: buy the existing portfolio or only new positions?

Smart Sync is a spot-only toggle with two very different behaviours.

Turn it **on** and you buy, at market price, every spot asset the lead trader is currently holding. Turn it **off** and you only copy positions they open after you subscribe.

Official guidance is to look at the lead trader's current holdings before deciding. Open the profile and check what they are already sitting on. If the existing book is deep in profit and you would be buying at the top of their entry, leaving Smart Sync off lets you wait for their next position instead.

## Who should skip copy trading entirely

- **Anyone who wants one-click replication of a whole portfolio.** The 0.5% rule will drop entries, so your allocation will drift from the lead trader's.
- **Anyone unwilling to pay a profit share.** Up to 30% of gains goes to the person you copied. On spot, that is a real drag on a strategy you could have executed manually.
- **Anyone reading Win rate as a per-trade statistic.** You will pick traders for the wrong reason.
- **Anyone assuming they can hold through a lead trader's exit.** When the lead trader sells, your position sells. Staying in requires you to have sold manually first or set your own take-profit and stop-loss.
- **Anyone who cannot see the lead trader's liquidation price.** You cannot. That information is not exposed to copy traders, which is one more argument for starting on the unleveraged spot side.

## FAQ

**Can I add leverage to spot copy trading?**
No. Spot copy trading has no leverage and no liquidation risk. Leverage exists only on the futures copy trading side, where you set it per contract.

**Can I see the lead trader's liquidation price?**
No. Copy traders cannot view the liquidation price of a lead trader's account.

**Can a lead trader copy other traders?**
No. Lead traders cannot join copy trading themselves.

**When exactly is the profit share taken?**
It is withheld from each profitable sell after trading fees, then recalculated against your full week's net PnL and settled every Monday at 00:00 (UTC+8). Excess withholding is refunded. Settlement is deferred while you still have ongoing copies open with that trader.

**Why are the coins I copied frozen?**
Spot copy purchases are frozen and unavailable for other uses until you sell them. You can see them under your assets.

**Is there a minimum order size?**
On spot, the minimum varies by coin and moves with price, so check the asset details on the manual trading page. On futures, the minimum is 10 USDT per order.

## Pick by situation, then check three things before you click Copy

If you want exposure to a skilled spot trader without liquidation risk, use **Spot copy trading with a fixed amount** and a Maximum total amount you would be comfortable losing entirely. Small fixed orders also let you observe the 0.5% rule in action within a few days.

If you already trade perpetuals and understand margin calls, futures copy trading is available with the same interface, but set leverage under 20x and cap the total.

Before confirming any copy, verify three numbers on screen: the coin's current minimum order size, the profit-sharing ratio that specific lead trader charges, and the settlement window you will be operating in. Those three determine what you actually keep.

👉 [Open OKX and set up your first copy trade](https://okx.com/join/CASH20)
