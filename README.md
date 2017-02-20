# Usage

#### Detailed documentation
``
$ man crontab
``


```
# Edit cronjobs schedule
$ crontab -e

# list all cronjobs
$ crontab -l
  Minute   Hour   Day of Month       Month          Day of Week        Command         output log
  (0-59)  (0-23)     (1-31)    (1-12 or Jan-Dec)  (0-6 or Sun-Sat)
    0        2          12             *                *            /usr/bin/find   >>  output.log
```

## Alternative first five fields
```
string         meaning
------         -------
@reboot        Run once, at startup.

@yearly        Run once a year, "0 0 1 1 *".

@annually      (same as @yearly)

@monthly       Run once a month, "0 0 1 * *".

@weekly        Run once a week, "0 0 * * 0".

@daily         Run once a day, "0 0 * * *".

@midnight      (same as @daily)

@hourly        Run once an hour, "0 * * * *".
```
