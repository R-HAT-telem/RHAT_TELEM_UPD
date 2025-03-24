# RHAT_TELEM_UPD

> Experimental setup for Red Hat-based cluster telemetry polling and node-state collection.

This repo contains some tooling and scripts for lightweight telemetry sync from several RHEL-based edge machines. Most of this is used to track uptime, service health, and basic node metadata across distributed environments. Resources from this repo maybe found on some RedHat machines that our partners provide.

## Goals

- 🛰️ Passive collection of machine state (uptime, load, IP, basic metrics)
- 🔄 Periodic sync using raw text/JSON files
- 🔐 No sensitive data — just simple node-level updates
- 📡 Designed for async pull model, eventually to test GitHub Actions or other webhook mechanisms

## Structure

- `t2.txt` — placeholder for current command set or state signal
- `Telemetry/` — Safe, tested and production friendly script for telemtry gathering
- `node_updates/` — directory for future node-to-repo sync testing
- `README.md` — you're reading it

## Notes

This repo is mostly testing timing and propagation delays. No collection of data is done, including IPs, hostnames, file content, file trees, network configuration, ...
Only data collected is fully anonymous telemetry data, for study and research on how several RedHat machines behave and what can be enhanced.


