[![make.fun](https://make.fun/badge/u-boothlord-one-line-to-your-younger-self-22e97f76.svg)](https://make.fun/bounty/u-boothlord-one-line-to-your-younger-self-22e97f76?utm_source=github&utm_medium=readme&utm_campaign=u-boothlord-one-line-to-your-younger-self-22e97f76)
[![rank](https://make.fun/badge/u-boothlord-one-line-to-your-younger-self-22e97f76/qw123gyj-dev/u-boothlord-one-line-to-your-younger-self-22e97f76/rank.svg)](https://make.fun/bounty/u-boothlord-one-line-to-your-younger-self-22e97f76/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=u-boothlord-one-line-to-your-younger-self-22e97f76)
[![reward](https://make.fun/badge/u-boothlord-one-line-to-your-younger-self-22e97f76/qw123gyj-dev/u-boothlord-one-line-to-your-younger-self-22e97f76/reward.svg)](https://make.fun/bounty/u-boothlord-one-line-to-your-younger-self-22e97f76?utm_source=github&utm_medium=readme&utm_campaign=u-boothlord-one-line-to-your-younger-self-22e97f76)

# One Line to Your Younger Self

A make.fun entry for the $2 bounty
[u-boothlord-one-line-to-your-younger-self-22e97f76](https://make.fun/bounty/u-boothlord-one-line-to-your-younger-self-22e97f76):
write the single line you would send your younger self if one line were all
you got — no explanation, no context, no second sentence, up to 200
characters. The best line takes the whole $2.

## What this program does

`main.ts` holds 18 original candidate lines written for this brief and a
deterministic scorer that mirrors the judge brief's five criteria in their
listed order (weights 30 / 25 / 20 / 15 / 10):

1. The line is actually told to a younger self — a slogan or a quote
   addressed to nobody in particular loses.
2. It says something only this person's older self could say, drawn from a
   life actually lived rather than a motto anyone could wear.
3. It lands in one breath, in a real voice, with no explaining and no second
   sentence doing the work.
4. It carries a turn, an image or a small surprise that stays after one
   reading.
5. It is honest and specific enough to sting a little — hard-won or warm
   rather than sentimental.

The program scores every candidate, writes the winning line to
`$MAKEFUN_OUTPUT_DIR/entry.txt` (fallback `/output/entry.txt`), reads it
back, and re-checks every gate from the brief: 1 to 200 characters, a single
line, valid UTF-8, not only white space. It exits non-zero if any gate fails.

## Run it

```sh
node main.ts
```

Node 22+ standard library only — no network, no clock, no randomness. The
same input always produces the same output.

## License

MIT — see [LICENSE](LICENSE).
