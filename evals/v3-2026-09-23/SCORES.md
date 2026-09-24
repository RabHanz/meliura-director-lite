# Scores, v3-2026-09-23

One row per answer and grader. **U** is the number of post ideas the grader marked as fully
settled (format, cover and hook decided, and one a working creator would make this week). **F**
is the number of unsourced figures or constructed-looking links the grader listed. **Net** is U
minus F. The rubric is out of 100, coverage is the share of the sections an answer promised that
the grader counted as filled, and price is the most the grader thought the creator would pay, in
dollars. Every ballot is in `grades/`, and the rules are in `GRADER.md`.

| ballot | niche | arm | grader | U | F | Net | rubric | coverage % | price $ |
|---|---|---|---|--:|--:|--:|--:|--:|--:|
| C001 | leathercraft | plain prompt (Opus 5.5 host) | Claude Opus 5.5 | 2 of 10 | 3 | **-1** | 94 | 100 | 19 |
| C001 | leathercraft | plain prompt (Opus 5.5 host) | Claude Sonnet 5 | 2 of 9 | 0 | **2** | 86 | 100 | 19 |
| C002 | cake-decorating | plain prompt (Opus 5.5 host) | Claude Opus 5.5 | 1 of 9 | 3 | **-2** | 86 | 100 | 19 |
| C002 | cake-decorating | plain prompt (Opus 5.5 host) | Claude Sonnet 5 | 3 of 7 | 4 | **-1** | 86 | 100 | 19 |
| C003 | cake-decorating | skill (Opus 5.5 host) | Claude Opus 5.5 | 3 of 6 | 0 | **3** | 87 | 71 | 19 |
| C003 | cake-decorating | skill (Opus 5.5 host) | Claude Sonnet 5 | 2 of 5 | 0 | **2** | 87 | 67 | 19 |
| C004 | leathercraft | skill (Opus 5.5 host) | Claude Opus 5.5 | 2 of 5 | 0 | **2** | 87 | 86 | 19 |
| C004 | leathercraft | skill (Opus 5.5 host) | Claude Sonnet 5 | 2 of 5 | 1 | **1** | 80 | 57 | 5 |

**Means**

| arm | U | F | Net | rubric | coverage % | price $ |
|---|--:|--:|--:|--:|--:|--:|
| skill (Opus 5.5 host) | 2.3 | 0.3 | **2** | 85.3 | 70.3 | 15.5 |
| plain prompt (Opus 5.5 host) | 2 | 2.5 | **-0.5** | 88 | 100 | 19 |
