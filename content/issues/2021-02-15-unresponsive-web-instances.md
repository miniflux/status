---
title: Unresponsive Web Instances
date: 2021-02-15 13:00:00-08:00
resolved: true
resolvedWhen: 2021-02-15 17:25:00-08:00
# Possible severity levels: down, disrupted, notice
severity: disrupted
affected:
  - reader
section: issue
---

The number of Goroutines spiked due to the activity of some large users.

The processes were unresponsive due to the number of file descriptors.
