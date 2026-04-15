---
layout: post
title: "Debugging under pressure without losing the thread"
date: 2026-04-15 08:15:00 -0700
categories: [Operations, Engineering]
image: /assets/covers/debugging.svg
---

High-pressure debugging gets chaotic fast. The instinct is to try everything at once, but that usually makes the timeline harder to trust.

My current rule is simple:

1. Freeze scope.
2. Reproduce once.
3. Change one variable at a time.
4. Write down what changed and what didn't.

The notes matter as much as the fix. They become the first draft of the incident write-up and save hours when a related issue appears later.
