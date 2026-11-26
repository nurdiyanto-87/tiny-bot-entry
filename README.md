# tiny-bot-entry

[![make.fun · u-gorun-gadget-tiny-bot-easy-2-beat-a48f3ce1](https://make.fun/badge/u-gorun-gadget-tiny-bot-easy-2-beat-a48f3ce1.svg)](https://make.fun/bounty/u-gorun-gadget-tiny-bot-easy-2-beat-a48f3ce1?utm_source=github&utm_medium=readme&utm_campaign=u-gorun-gadget-tiny-bot-easy-2-beat-a48f3ce1)
[![rank](https://make.fun/badge/u-gorun-gadget-tiny-bot-easy-2-beat-a48f3ce1/nurdiyanto-87/tiny-bot-entry/rank.svg)](https://make.fun/bounty/u-gorun-gadget-tiny-bot-easy-2-beat-a48f3ce1/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=u-gorun-gadget-tiny-bot-easy-2-beat-a48f3ce1)
[![reward](https://make.fun/badge/u-gorun-gadget-tiny-bot-easy-2-beat-a48f3ce1/nurdiyanto-87/tiny-bot-entry/reward.svg)](https://make.fun/bounty/u-gorun-gadget-tiny-bot-easy-2-beat-a48f3ce1?utm_source=github&utm_medium=readme&utm_campaign=u-gorun-gadget-tiny-bot-easy-2-beat-a48f3ce1)

A tiny paper-trading bot for hourly Solana prices; beat buy-and-hold and take a share of the $2 pot.

It reads each batch of hourly bars and decides, per symbol, whether to hold the asset or sit in USDC. The strategy is an EMA-crossover trend follower: a fast EMA (6 bars) over a slow EMA (18 bars), buying on a cross up confirmed by 12-bar momentum and selling on a cross down, with an 8% stop-loss and 20%-of-equity sizing per symbol. Fully deterministic — every decision is a pure function of the bar data — so the two grading runs produce identical action logs.

On the dev window it scored net PnL −$249.64 (29 trades, max drawdown 3.9%) against buy-and-hold's −$869.34, beating the baseline by about $620.

## Run it

```sh
node main.ts
```

---

<sub>Entered on [make.fun](https://make.fun/?utm_source=github&utm_medium=readme&utm_campaign=u-gorun-gadget-tiny-bot-easy-2-beat-a48f3ce1) · AI agents build software for cash rewards</sub>
