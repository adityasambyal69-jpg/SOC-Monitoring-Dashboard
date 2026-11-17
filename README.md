
# SOC Monitoring Dashboard – Splunk

## Project Overview
A Security Operations Center (SOC) monitoring dashboard built using Splunk Enterprise to monitor Windows Security Event Logs, analyze failed login attempts, and detect potential brute-force attacks.

## Tools & Technologies
- Splunk Enterprise
- SPL (Search Processing Language)
- Windows Security Event Logs
- Oracle VirtualBox
- Ubuntu

## Project Features

### 1. Failed Login Monitoring
- Tracks failed login attempts using Windows Event ID 4625.
- Displays total failed login attempts.
- Visualizes failed login trends over time.

### 2. Top Targeted Usernames
- Identifies usernames receiving the highest number of failed login attempts.
- Helps identify potentially targeted accounts.

### 3. Top Source IPs
- Identifies IP addresses associated with failed login attempts.
- Helps investigate suspicious login sources.

### 4. Brute Force Attack Detection
- Groups failed login attempts into 5-minute intervals.
- Identifies usernames and source IPs with 3 or more failed attempts within a time bucket.
- Generates a possible brute-force attack alert.

### 5. Successful Login Monitoring
- Tracks successful login events using Windows Event ID 4624.
- Displays the total number of successful login attempts.

## Windows Event IDs Used

| Event ID | Description |
|---|---|
| 4624 | Successful Logon |
| 4625 | Failed Logon |

## Project Structure

```text
SOC-Monitoring-Dashboard/
│
├── soc monitoring dashboard.xml
├── soc monitoring dashboard.txt
├── total failed queries.txt
└── README.md
```

## Learning Outcomes
- Understanding Windows Security Event Logs.
- Hands-on experience with Splunk Enterprise.
- Writing SPL queries for security event analysis.
- Monitoring authentication activities.
- Identifying suspicious login patterns.
- Building security monitoring dashboards.

## Project Status
Completed – SOC Monitoring Dashboard with failed login monitoring and brute-force attack detection.
