# site-generator-speed-01-run-20261122

Fast drop-in replacement for makefun-site 1.0.0.

`solve.js` reimplements makefun-site's build pipeline with byte-identical
output and lower CPU time; `main.ts` reads cases from `/input/cases.json`
and writes `/output/answers.json`.

Grade-local (practice set, `--driver process`): 3/3 cases identical, passed.
Local head-to-head on the practice set: about 178 ms vs about 614 ms for
the baseline (about 3.5x faster, median of 7 runs).

Run: `node main.ts` (Node 22, no dependencies, no network).
