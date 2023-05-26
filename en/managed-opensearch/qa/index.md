---
title: "{{ mos-name }}. Questions and answers"
description: "How do I get the logs of my activity in {{ OS }}? Find the answer to this and other questions in this article."
---

# Questions and answers about {{ mos-name }}

## General questions {#general}

#### How are {{ OS }} clusters maintained? {#service-window}

Maintenance in {{ mos-short-name }} implies:

* Automatic installation of {{ OS }} updates and fixes for your database hosts.
* Changes to the host class and storage size.
* Other {{ mos-short-name }} maintenance activities.

For more information, see [Maintenance](../concepts/maintenance.md).

#### Is cluster backup enabled by default? {#default-backup}

Yes, backup is enabled by default. For {{ mos-name }} clusters, a complete backup is performed once a day, and all the indexes are saved. This helps restore a cluster's state from any available backup.

Backups are kept for 7 days.

#### Which version of {{ OS }} does {{ mos-short-name }} use? {#dbms-version}

The {{ OS }} versions maintained by the vendor are available in {{ mos-short-name }}.

#### What happens when a new {{ OS }} version is released? {#new-version}

When new versions include only bug fixes (such versions are called _maintenance releases_), the cluster software is automatically updated after a short testing period.

The owners of the affected DB clusters receive advanced notice of expected work times and DB availability.

#### What happens when the {{ OS }} version becomes deprecated? {#dbms-deprecated}

{{ mos-short-name }} automatically notifies cluster owners by email that their {{ OS }} version is approaching end of life.

Clusters running the {{ OS }} version that is no longer supported are automatically upgraded to the most up-to-date and stable maintained version.

The owners of the affected clusters receive advanced notice of expected work times and DB availability.

{% include [logs](../../_qa/logs.md) %}

{% include [log-duration](../../_includes/mdb/log-duration-qa.md) %}

#### How do I set up an alert that is triggered once a certain disk space percentage is used up? {#disk-space-percentage}

[Create an alert](../../managed-opensearch/operations/monitoring.md#monitoring-integration) with the `disk.used_bytes` metric in {{ monitoring-full-name }}. This metric shows the disk space usage in the {{ mos-name }} cluster.

For `disk.used_bytes`, use notification thresholds. Here are their recommended values:

* `Alarm`: 90% of disk space.
* `Warning`: 80% of disk space.

The thresholds are only set in bytes. For example, here are the recommended values for a disk of 100 GB:

* `Alarm`: `96636764160` bytes (90%).
* `Warning`: `85899345920` bytes (80%).