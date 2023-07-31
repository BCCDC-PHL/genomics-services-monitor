# Genomics Services Monitor

A tool for monitoring a set of [systemd](https://systemd.io/)-based services and feeding their status to the [BCCDC-PHL Genomics Services Monitor Site](https://github.com/BCCDC-PHL/genomics-services-monitor-site). 

## Usage
```
usage: genomics-services-monitor [-h] [--services-list SERVICES_LIST] [--service-status-output SERVICE_STATUS_OUTPUT] [--scan-interval-seconds SCAN_INTERVAL_SECONDS]

optional arguments:
  -h, --help            show this help message and exit
  --services-list SERVICES_LIST
  --service-status-output SERVICE_STATUS_OUTPUT
  --scan-interval-seconds SCAN_INTERVAL_SECONDS
```

The `--services-list` file should be a simple text file with the name of a systemd service on each line. The `--service-status-output` is a json-format file where the status of each service will be written to. The `--scan-interval-seconds` controls how often the status of each service will be checked. 
