---
title: Unresponsive Web Instances
date: 2021-02-18 00:30:00-08:00
resolved: true
resolvedWhen: 2021-02-18 07:24:00-08:00
# Possible severity levels: down, disrupted, notice
severity: disrupted
affected:
  - reader
section: issue
---

There is a recurring problem that makes the web instances unresponsive.

The number of file descriptors increased suddenly. As result, users cannot use the service anymore.

Unfortunately, this problem happened overnight in PST time zone.

__The root cause is not identified yet. Restarting the instances solve the issue temporarily.__

Investigation still in progress.

![Grafana - File Descriptors](/images/2021-02-18-file-descriptors.png)
