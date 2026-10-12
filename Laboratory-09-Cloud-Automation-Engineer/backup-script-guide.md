
# Backup Script Guide

## 1. Backup Script Code

The following Bash script creates a compressed backup of the application data directory and includes a timestamp in the filename.

```bash
#!/bin/bash
# Automated Backup Script for CloudNova Technologies

SOURCE_DIR="app-data"
BACKUP_DIR="backups"
TIMESTAMP=$(date +"%Y%m%d_%H%M%S")

echo "Initiating automated backup..."

# Create the backup directory if it does not exist
mkdir -p $BACKUP_DIR

# Compress the source directory into a tarball (.tar.gz)
tar -czf $BACKUP_DIR/backup_$TIMESTAMP.tar.gz $SOURCE_DIR

echo "Backup completed successfully at $TIMESTAMP!"
```

## 2. File Permissions

Command used:

```bash
chmod +x backup.sh
```

The `chmod +x` command gives the script executable permission, allowing it to run as a program instead of requiring it to be opened manually in a text editor.

## 3. Cron Job Configuration

Cron expression used:

```cron
0 2 * * * /root/backup.sh
```

This schedules the backup script to run every day at 2:00 AM.

### Breakdown of the Five Time Fields

| Field | Value | Meaning |
|---|---|---|
| Minute | 0 | At minute zero |
| Hour | 2 | At 2 AM |
| Day of Month | * | Every day of the month |
| Month | * | Every month |
| Day of Week | * | Every day of the week |

The `/root/backup.sh` portion specifies the path to the script that Cron executes.

