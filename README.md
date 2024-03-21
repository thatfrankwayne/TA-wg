![icon](static/appIcon_2x.png)

# TA-wg

A Splunk technology add-on (TA) to collect and parse WireGuard logs.

## Purpose

The TA ingests and parses WireGuard debug log events.
WireGuard kernel log events written to `/var/log/wireguard` are indexed.
TA-wg parses those events at search time and adds various metadata fields.

## Prerequisites and Dependencies

The TA requires a **Linux operating system**. 
The instructions (in Splunkbase) assume that systemd, systemd-journald and rsyslog are used on the monitored distribution.

## Developer

The TA was developed by Frank Wayne.

## Support Contact

Contact [the developer](mailto:frank.wayne@northwestern.edu?subject=TA-wg) with questions, bug reports or change requests. You can also refer or contribute to the [GitHub repository](https://github.com/thatfrankwayne/TA-wg).
