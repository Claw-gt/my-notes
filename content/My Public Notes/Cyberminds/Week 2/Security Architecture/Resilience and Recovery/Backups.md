Provide a data safety net

### Backup Media

- Tape backups
- Disk-to-disk backups
- Cloud backups

### Types

- **Full** Backup
	-Snapshots
	-Images
- **Differential** Backup: data modified since last full backup
- **Incremental** Backup: all data modified since the last full or **incremental** backup (consumes less space than differential)
- **Journaling**: records a transaction log of changes

Balance time and cost of performing backups with the potential for data loss

### ⚠ Encrypt Bakups

---

# Restoring backups

The order of restoration is important
Prioritize most important services

**Non-persistence** allows us to back up only unique data