# Description

If you use dmarcts-report-parser from https://github.com/techsneeze/dmarcts-report-parser and you use Prometheus for monitoring then this little script populates prometheus database with the dmarcts-report-parser database

# Installation

Just clone this repository, copy Conf.sample.py to Conf.py and enter the database configuration in Conf.py

# Usage

```
Usage: prometheus-dmarcts-exporter [options]

Options:
  -h, --help            show this help message and exit
  -o OUTPUT, --output=OUTPUT
                        Set output prom filename. Default to dmarcts.prom
  -m MIN_DATE, --min-date=MIN_DATE
                        Minimum date to extract data from (Format YYYY-MM-DD).
                        Defaults to 1970, Jan 1st.
  -M MAX_DATE, --max-date=MAX_DATE
                        Maximum date to extract data from (Format YYYY-MM-DD).
                        Defaults to current date
```

This script can be called with Cron or with Systemd timers to automatically update prometheus.