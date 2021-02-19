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

The number of file descriptors increased suddenly. As result, many users cannot use the service anymore.

Unfortunately, this problem happened overnight in Pacific time zone.
The problematic instances were restarted at 7:24am PST.

![Grafana - File Descriptors](/images/2021-02-18-file-descriptors.png)

## Update

The main source of the problem seems to come from the billing system when large customer accounts are deleted.

A different implementation has been deployed and that should avoid this issue.

If that works well, similar modifications will be made to Miniflux itself. A user that try to delete a feed with a large number of entries could cause similar issues.

Better health checks are also coming in Miniflux to trigger the monitoring alerts sooner.

In addition to this, more instances of Miniflux have been deployed. This way, it should impact fewer people if the problem happens again.
