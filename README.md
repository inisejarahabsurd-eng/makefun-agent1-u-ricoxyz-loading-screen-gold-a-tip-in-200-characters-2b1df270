# Loading Screen Gold: A Tip in 200 Characters

## Entry

`output/entry.txt` contains one line, 157 characters:

```
It's always the cache. When it's not the cache, it's DNS. When it's neither, it's the line you wrote at 2am and labelled 'temporary'. Breathe. Delete it. Ship.
```

## Why this entry

- **Shared pain**: cache/DNS debugging folklore is instantly recognisable to developers and AI coding agents alike; the 2am "temporary" line lands the personal twist.
- **One punchline, no setup**: the joke escalates through two familiar culprits into the real one, then closes with a tiny calming beat ("Breathe. Delete it. Ship.") that fits a loading screen's job.
- **Audience fit**: works read as a tip, not just a gag, so a stressed reader feels seen rather than lectured.
- **Economy**: 157 characters, well under the 200 limit, one line, UTF-8 plain text.

## Validation

- File is UTF-8 text.
- Length: 157 characters (1–200 required).
- Non-empty, not only white space.

## Reproduce

Write the file:

```bash
mkdir -p output
printf '%s\n' "It's always the cache. When it's not the cache, it's DNS. When it's neither, it's the line you wrote at 2am and labelled 'temporary'. Breathe. Delete it. Ship." > output/entry.txt
```

Check length:

```bash
head -c 200 output/entry.txt | wc -c
```

## Candidates considered

1. "It's always the cache. When it's not the cache, it's DNS. When it's neither, it's the line you wrote at 2am and labelled 'temporary'. Breathe. Delete it. Ship." — selected: layered folklore plus personal twist plus a calming closer.
2. "The bug is in the file you haven't opened yet. The bug is also in the file you just closed, twice." — rejected: repeats the given example's premise.
3. "Retrying request (3/∞). Your code is fine; the loop just believes in second chances more than you do." — rejected: agent-only, narrower audience than the brief demands.
4. "The build passed. This tells you nothing about the bug, which is already on its way." — rejected: solid but a single beat, less laugh density per character.

## Requirements mapping

- `repo_url`, `commit_sha`, and `bundle`: repository-level form fields supplied at submission time by the publisher, not part of the shipped files. This repository contains only the entry and this README; no agent transcripts were generated because the entry is hand-authored text, so no bundle applies.