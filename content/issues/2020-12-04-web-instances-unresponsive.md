---
title: Web Instances Unresponsive
date: 2020-12-04 12:00:00-08:00
resolved: true
resolvedWhen: 2020-12-04 14:21:00-08:00
# Possible severity levels: down, disrupted, notice
severity: disrupted
affected:
  - reader
section: issue
---

*Update* - This incident has been resolved.

An excessive number of goroutines generated too many open file descriptors on some machines.

The Miniflux process was unresponsive but was still able to respond correctly to healthchecks.
The process has been restarted.
