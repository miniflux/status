---
title: Bad Gateway / Docker Crash
date: 2021-04-06 01:04:10-07:00
resolved: true
resolvedWhen: 2021-04-06 08:09:09-07:00
# Possible severity levels: down, disrupted, notice
severity: down
affected:
  - reader
  - workers
  - billing
section: issue
---

The Docker daemon crashed. The problem seems related to Docker logs rotation.
Containers were still running but the overlay network was broken.

Docker has been completely reinstalled and the applications have been redeployed.

Monitoring checks reported the problem as expected but, unfortunately, I was sleeping :(

This outage created a long period of downtime for people in the opposite time zone.
