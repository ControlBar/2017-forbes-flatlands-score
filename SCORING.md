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

> ../../bin/align-time --file=forbes2017.comp-input.yaml
Reading competition from 'forbes2017.comp-input.yaml'
Reading flying time range from 'forbes2017.cross-zone.yaml'
Reading zone tags from 'forbes2017.tag-zone.yaml'
Aligning times completed in 39.12 m

> ../../bin/discard-further --file=forbes2017.comp-input.yaml
Reading competition from 'forbes2017.comp-input.yaml'
Reading task length from 'forbes2017.task-length.yaml'
Reading zone tags from 'forbes2017.tag-zone.yaml'
Filtering times completed in 1.17 m

> ../../bin/mask-track --file=forbes2017.comp-input.yaml
Reading competition from 'forbes2017.comp-input.yaml'
Reading task length from 'forbes2017.task-length.yaml'
Reading flying time range from 'forbes2017.cross-zone.yaml'
Reading zone tags from 'forbes2017.tag-zone.yaml'
Masking tracks completed in 58.30 s

> ../../bin/land-out --file=forbes2017.comp-input.yaml
Reading land outs from 'forbes2017.mask-track.yaml'
Land outs counted for distance difficulty completed in 93.54 ms

> ../../bin/gap-point --file=forbes2017.comp-input.yaml
Reading pilots absent from task from 'forbes2017.comp-input.yaml'
Reading pilots that did not fly from 'forbes2017.cross-zone.yaml'
Reading start and end zone tagging from 'forbes2017.tag-zone.yaml'
Reading masked tracks from 'forbes2017.mask-track.yaml'
Reading distance difficulty from 'forbes2017.land-out.yaml'
Tallying points completed in 972.13 ms
```
