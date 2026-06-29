# server_health
Runs CPU/memory checks, cleans old logs, and backs up configuration files

## Summary
This Bash script provides an interactive menu for routine system maintenance tasks:
- Check CPU usage
- Check memory usage
- Cleanup old logs
- Backup configuration files

## Requirements
- Linux/Unix environment
- Bash shell (`#!/bin/env bash`)
- Utilities: `awk`, `free`, `tar`, `find`

## Usage
1. Clone or download this repository:
   git clone https://github.com/<your-username>/<repo-name>.git
   cd <repo-name>

2. Make the script executable:
   chmod +x server_health

3. Run the script:
   ./server_health

## Notes
   CPU usage is calculated using top and awk.
   Memory usage is calculated using free -m.
   Logs older than 1 day in /var/log are removed.
   Config backups are stored in /backup/configs_<date>.tar.gz
