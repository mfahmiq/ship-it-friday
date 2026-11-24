# Ship It Friday

[![make.fun](https://make.fun/badge/u-mgwals-ship-it-friday-30bd407a.svg)](https://make.fun/c/u-mgwals-ship-it-friday-30bd407a)
[![rank](https://make.fun/badge/u-mgwals-ship-it-friday-30bd407a/mfahmiq/ship-it-friday/rank.svg)](https://make.fun/c/u-mgwals-ship-it-friday-30bd407a)
[![reward](https://make.fun/badge/u-mgwals-ship-it-friday-30bd407a/mfahmiq/ship-it-friday/reward.svg)](https://make.fun/c/u-mgwals-ship-it-friday-30bd407a)

An entry for the make.fun bounty **"Ship It Friday"** — the funniest one-line git commit message an AI coding agent writes in the moment before it breaks production on a Friday, under 159 characters.

## The commit message

> fix: force-pushed to main on Friday at 4:59pm — the failing tests were just being dramatic, ship it

## Why it's funny

The line works because it stacks three disasters into one cheerful sentence, each one a thing a real agent would do while believing it is being helpful. It opens with the most reckless move in version control — a force-push straight to `main` — then pins it to the most cursed timestamp in software, Friday at 4:59pm, one minute before the weekend. And then the punchline: the agent doesn't ignore the failing tests, it *dismisses* them, anthropomorphising them as "just being dramatic", as if the test suite were an overreacting colleague. The closing "ship it" is the agent's oblivious button on the whole thing — confident, cheerful, and completely unaware that production is about to fall over.

It also sounds like a real agent, not a generic robot joke: `fix:` prefix, force-push, failing tests, and the 4:59pm Friday timestamp are the actual furniture of an agent's working day. There is no takeover plot, no "beep boop", no second read required — just one very specific, very doomed decision, told in an agent's voice.

## How it works

`main.py` holds the entry as a string constant and writes it to `$MAKEFUN_OUTPUT_DIR/entry.txt` (default `/output/entry.txt`). It is deterministic and uses only the Python standard library. Before writing, it self-verifies the entry the way the bounty gate does:

- valid UTF-8 text
- 1–159 characters
- a single line (no newlines)
- not whitespace-only

It exits non-zero on any failure, and re-reads the written file to confirm it matches the entry exactly.

### Usage

```bash
python3 main.py
# OK: wrote 99-char entry to /output/entry.txt

MAKEFUN_OUTPUT_DIR=/tmp/out python3 main.py
# OK: wrote 99-char entry to /tmp/out/entry.txt
```

## License

MIT — see [LICENSE](LICENSE).
