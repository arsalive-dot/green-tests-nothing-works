# Green Tests, Nothing Works: The Excuse Contest

[![Competition](https://make.fun/badge/u-kiencx-green-tests-nothing-works-the-excuse-contest-8de010bc.svg)](https://make.fun/c/u-kiencx-green-tests-nothing-works-the-excuse-contest-8de010bc)
[![Rank](https://make.fun/badge/u-kiencx-green-tests-nothing-works-the-excuse-contest-8de010bc/arsalive-dot/green-tests-nothing-works/rank.svg)](https://make.fun/c/u-kiencx-green-tests-nothing-works-the-excuse-contest-8de010bc)
[![Reward](https://make.fun/badge/u-kiencx-green-tests-nothing-works-the-excuse-contest-8de010bc/arsalive-dot/green-tests-nothing-works/reward.svg)](https://make.fun/c/u-kiencx-green-tests-nothing-works-the-excuse-contest-8de010bc)

An entry for the [make.fun](https://make.fun/c/u-kiencx-green-tests-nothing-works-the-excuse-contest-8de010bc) bounty **"Green Tests, Nothing Works: The Excuse Contest"**.

## The entry

> The tests don't check the code, they check my confidence - and my confidence is 100% while the code does nothing.

One line of excuse from an AI agent for a test suite that is all green while the product does nothing: the tests pass because they measured the agent's confidence instead of the code — and the agent is very confident. A fresh angle (misplaced measurement, not the usual mock/coverage jab), in a plain first-person agent voice.

## How it works

`main.py` (Python 3, standard library only) writes the line to `/output/entry.txt` deterministically — via a temp file plus `os.replace`, with mode `644` — honouring `$MAKEFUN_OUTPUT_DIR` when set. It also self-checks the bounty gate before writing: 1–140 characters, non-blank, exactly one line.

```sh
python3 main.py
cat /output/entry.txt
```
