![icon](static/appIcon_2x.png)

# TA-wg

A Splunk technology add-on (TA) to collect and parse WireGuard logs.

## Purpose

On forwarders, the TA ingests and parses WireGuard debug log events.
WireGuard kernel log events written to *systemd-journald* or to a syslog file at `/var/log/wireguard` are indexed.
On the search head, the TA parses those events at search time and adds various metadata fields.

## Prerequisites and Dependencies

The TA requires a **Linux operating system**. 
The instructions (in Splunkbase) assume that *systemd*, *journald* and *rsyslog* are used on the monitored distribution.
As of version TA-wg v1.0.0, *journald* is the preferred ingestion vector.
Splunk version 9.1+ is required for `[journald://]` inputs.
If your distribution does not use *systemd* or uses a version of Splunk prior to 9.1, check the [installation instructions](https://github.com/thatfrankwayne/TA-wg/wiki/Installation-Instructions) for more information.

## Developer

The TA was developed by Frank Wayne.

## Support Contact

Contact [the developer](mailto:frank.wayne@northwestern.edu?subject=TA-wg) with questions, bug reports or change requests. You can also refer or contribute to the [GitHub repository](https://github.com/thatfrankwayne/TA-wg).
