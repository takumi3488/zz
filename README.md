# zzsleep

A CLI sleep/timer utility that waits until a specified duration or time. Installs as the `zz` binary.

## Installation

```sh
cargo install zzsleep
```

This installs the binary as `zz`.

## Usage

```
zz <duration|time>
```

### Duration

```sh
zz 10          # wait 10 seconds
zz 2h          # wait 2 hours
zz 5m          # wait 5 minutes
zz 30s         # wait 30 seconds
zz 2h 5m 30s   # wait 2 hours, 5 minutes, and 30 seconds
```

### Wait until a specific time

```sh
zz 12:30             # wait until 12:30 (next occurrence today or tomorrow)
zz 12:30:45          # wait until 12:30:45
zz 20260220T123000+0900   # wait until 2026-02-20 12:30:00 JST (ISO 8601)
zz 20260220T123000Z       # wait until 2026-02-20 12:30:00 UTC (ISO 8601)
```
