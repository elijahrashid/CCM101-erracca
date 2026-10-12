
# Mission 9: The Cloud Automation Engineer

## Mission Overview

This mission focuses on automating repetitive cloud administration tasks using Bash scripting and Cron. I created a sample application data directory, developed a script to compress the data into a backup file, and configured a scheduled task to run the script automatically.

## Objectives

- Understand Bash scripts and variables.
- Create a script that backs up application data.
- Use chmod to make a script executable.
- Verify that the script creates a compressed backup.
- Configure a Cron job to run the script every day at 2:00 AM.
- Document the automation process using Markdown.

## Commands Executed

```bash
mkdir app-data
echo "This is critical client data." > app-data/data.txt
nano backup.sh
./backup.sh
chmod +x backup.sh
ls -l backups/
crontab -l
env EDITOR=nano crontab -e
```

## Skills Learned

- Writing and executing Bash scripts.
- Using variables in automation.
- Creating compressed backups with tar.
- Managing file permissions with chmod.
- Scheduling recurring tasks using Cron.
- Documenting technical procedures in Markdown.
- Maintaining a GitHub cloud computing portfolio.

