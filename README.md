# Unraid User Scripts

Various bash scripts to be used in the User Scripts plugin in Unraid


## Backup Scripts

### backup_all_appdata

This script creates an individual tar file for each docker appdata directory found in your appdata path.  Furthermore, it stops and restarts each container before and after backup if the container was running at the time of the backup.

### backup_flashdrive

This script creates a dated tar file of the Unraid USB flash drive.

### backup_plex_db

This script stops the plex container and copies the main plex db file to a backup location of your choosing before restarting the container.

### backup_all_appdata

This script creates an individual tar.gz file for all the plexdata that you redirect to be outside of your regular plex appdata directory.  This is useful for making your appdata backups much smaller as to not capture directories like Media and Transcoder Cache that can take up huge amounts of space but is not mission critical for most.

### backup_select_appdata

This script creates an invididual tar file for each docker appdata directory that you define (needs both container name and path to it's appdata).  Furthermore, it stops and restarts each container before and after backup if the container was running at the time of the backup.

## Usage

Create a new User script and paste script text in

### Example Cron Schedules

Cron schedule to run script every morning at 5:00am

```bash
0 5 * * *
```

Cron schedule to run script every Monday morning at 5:00am

```bash
0 5 * * 1
```

Cron schedule to run script every morning at 5:00am except Monday

```bash
0 5 * * 0,2-6
```
