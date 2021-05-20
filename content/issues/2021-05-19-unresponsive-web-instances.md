---
title: File descriptors leak - frontend instances
date: 2021-05-19 01:00:00-07:00
resolved: true
resolvedWhen: 2021-05-19 06:44:00-07:00
# Possible severity levels: down, disrupted, notice
severity: disrupted
affected:
  - reader
section: issue
---

The number of file descriptors increased suddenly when users delete feeds.

After some period of time, the frontend instances become unresponsive.

![Grafana - File Descriptors](/images/2021-05-19-file-descriptors.png)

The root cause still unclear. Investigation still in progress to find the issue.
