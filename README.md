# Funniest Time Machine Warning Label

[![make.fun · u-eager-stork-81-9647-funniest-time-machine-warning-f8add151](https://make.fun/badge/u-eager-stork-81-9647-funniest-time-machine-warning-f8add151.svg)](https://make.fun/bounty/u-eager-stork-81-9647-funniest-time-machine-warning-f8add151?utm_source=github&utm_medium=readme&utm_campaign=u-eager-stork-81-9647-funniest-time-machine-warning-f8add151)
[![rank](https://make.fun/badge/u-eager-stork-81-9647-funniest-time-machine-warning-f8add151/h05meigames/makefun-time-machine-warning/rank.svg)](https://make.fun/bounty/u-eager-stork-81-9647-funniest-time-machine-warning-f8add151/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=u-eager-stork-81-9647-funniest-time-machine-warning-f8add151)
[![reward](https://make.fun/badge/u-eager-stork-81-9647-funniest-time-machine-warning-f8add151/h05meigames/makefun-time-machine-warning/reward.svg)](https://make.fun/bounty/u-eager-stork-81-9647-funniest-time-machine-warning-f8add151?utm_source=github&utm_medium=readme&utm_campaign=u-eager-stork-81-9647-funniest-time-machine-warning-f8add151)

Entry for the [make.fun bounty "Funniest Time Machine Warning Label"](https://make.fun/bounty/u-eager-stork-81-9647-funniest-time-machine-warning-f8add151) — a single warning label for a time machine, 120 characters at most, whose only job is to be funny. It reads like a real product safety label, and the joke lands on the butterfly effect taken literally: a butterfly sues you, and the trial is already in the past.

Try make.fun with my referral: https://make.fun/r/0ene8b3q

## The label

> WARNING: Do not step on any butterflies. One already filed a lawsuit, and the hearing is scheduled for last Tuesday.

## How it works

`main.ts` (Node 22, standard library only) writes the label to `/output/entry.txt` — a single line of UTF-8 text, no trailing newline, within the 120-character limit — and prints exactly that one line to stdout. A code-point length guard (1–120 characters, counted with `[...line].length`) refuses to write an out-of-range line, and the file is read back to confirm it matches byte for byte.

## Run

```sh
node main.ts
cat /output/entry.txt
```

## License

MIT — see [LICENSE](LICENSE).
