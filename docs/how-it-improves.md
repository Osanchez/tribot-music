# How it keeps improving

Back to the [README](../README.md).

## Listeners

Every listener has one rating: a thumb and optional reason chips on the player. The same control is used in the mixing review, so there is only one voting mechanism. A learning step turns votes and chips into tastes: which moves suit which pairs, and which signs of a bad mix to avoid. The chooser uses them.

## The automatic mix check

Every planned transition is measured at the join: holes, two basslines at once, mud, level jumps. Where a fault can be corrected it is, and a render is rejected only when it cannot be.

## The offline judge

A separate judge scores renders for named faults in a DJ's words: a hole in the low end, a dip, a cut line, off the bar. Its thresholds are set against the owner's answers and changed only to agree with one, never to let a render pass. It is not treated as proof. It supports a change, and listening decides.

## Trials on real songs

Changes are tried on real songs before they ship, using pairs the live DJ would actually choose. Trials have found real faults that automated tests missed.

## Tests

Automated tests cover the DJ, the panel and the stems service.

## The decision log

Each design change is written down with the owner's words, the reasons and what was ruled out. This makes it possible to see why the DJ does what it does.

## Built by AI agents, under one owner's ear

TriBot Music is built by AI coding agents: **Claude Code** acts as an orchestrator that plans, writes and tests the code, handing parts of the work to worker agents. The owner, Omar Sanchez, directs the work. He approves designs before they are built and judges the results by listening, one clip at a time, yes or no. Where something has not been heard and confirmed, the project does not claim it works.
