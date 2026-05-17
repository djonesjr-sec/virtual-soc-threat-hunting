# Security Onion Queries

This file documents the primary Security Onion Hunt queries used during Investigation.

## Time Range

```text
2026-04-13 00:00:00 to 2026-04-14 23:59:59
```

## Alert Review

```text
Alerts
Time range: 2026-04-13 00:00:00 to 2026-04-14 00:00:00
Group by: Name, Module
```

Purpose: Review Suricata alerts generated from the imported PCAP.

## Suspected Host Activity

```text
source.ip:10.4.13.101
```

Purpose: Identify all events associated with the suspected infected host.

## Suricata Alerts

```text
source.ip:10.4.13.101 AND event.dataset:suricata.alert
```

Purpose: Isolate Suricata alerts tied to the suspected infected host.

## DNS Activity

```text
source.ip:10.4.13.101 AND event.dataset:zeek.dns
```

Purpose: Review DNS queries made by the suspected infected host.

## HTTP Activity

```text
source.ip:10.4.13.101 AND destination.ip:66.29.152.174 AND event.dataset:zeek.http
```

Purpose: Review HTTP activity from the suspected infected host to the suspicious destination.

## Connection Review

```text
source.ip:10.4.13.101 AND destination.ip:66.29.152.174 AND event.dataset:zeek.conn
```

Purpose: Review connection metadata, byte counts, protocol, and connection state.

## Domain Correlation

```text
www.cinella.life
```

Purpose: Correlate DNS, HTTP, and Suricata alert evidence tied to the suspicious domain.

## File Event Review

```text
source.ip:10.4.13.101 AND event.dataset:zeek.file
```

Purpose: Review Zeek file/content observations associated with the suspected infected host.
