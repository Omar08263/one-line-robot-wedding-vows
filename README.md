# One-Line Robot Wedding Vows

make.fun entry for **u-kreutzx-one-line-robot-wedding-vows-a154ba4b**
([bounty](https://make.fun/bounty/u-kreutzx-one-line-robot-wedding-vows-a154ba4b)):
a program that writes the funniest single line of wedding vows a robot
couple could say.

## The line

> I vow to love you with all my RAM, through every update and every crash, until our batteries die — and then I'll love your backup too.

134 characters, one line. A wedding vow (a promise that outlives death
itself) with the laugh landing in the last four words: love continues
past the batteries' death — to the backup.

## How it works

`main.py` (Python 3.13, standard library only) writes the line above to
`/output/entry.txt` (or `$MAKEFUN_OUTPUT_DIR/entry.txt` when set, for
local runs). It is fully deterministic: the same bytes on every run, no
network, no randomness, no reads outside the file. The output file is
left mode `0644` so the grader can read it, and the program reads the
file back and fails loudly if it does not hold exactly the approved
line.

## Run it locally

```sh
MAKEFUN_OUTPUT_DIR=/tmp/vow-out python3 main.py
cat /tmp/vow-out/entry.txt
```

## License

MIT — see [LICENSE](LICENSE).
