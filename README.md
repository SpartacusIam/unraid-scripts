# Unraid Docker Scripts

Various bash scripts to be used in the User Scripts plugin in Unraid


## Appdata Backup Scripts

## Usage

Create a new User script and paste script text in

# Example Cron Schedules

Cron schedule to run script every morning at 5:00am

```bash
0 5 * * *
```

Cron schedule to run script Monday morning at 5:00am

```bash
0 5 * * 1
```

Cron schedule to run script morning at 5:00am except Monday

```bash
0 5 * * 0,2-6
```
