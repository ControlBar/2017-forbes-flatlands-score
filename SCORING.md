# Scoring Log

With this repo and [flare-timing](https://github.com/BlockScope/flare-timing)
cloned as siblings the following commands show how to score all tasks at once
for the **Forbes Flatlands 2017** competition.

```
> ../../bin/extract-input --file=forbes2017.fsdb
Extracted 6 tasks from "Forbes Flatlands 2017"
Extracting tasks completed in 1.40 s

> ../../bin/cross-zone --file=forbes2017.comp-input.yaml
Reading competition from 'forbes2017.comp-input.yaml'
Tracks crossing zones completed in 1.07 m

> ../../bin/task-length --file=forbes2017.comp-input.yaml
forbes2017.comp-input.yaml
Measuring task lengths completed in 3.35 m

> ../../bin/tag-zone --file=forbes2017.cross-zone.yaml
Reading zone crossings from 'forbes2017.cross-zone.yaml'
Tagging zones completed in 807.92 ms
```
