# 2. Secured and Monitored Web Infrastructure

## Overview

This infrastructure builds on the previous design and adds:
- Security: SSL encryption and firewalls
- Monitoring: real-time performance tracking

### Added components:
- 3 firewalls: one for Load Balancer, one per application server
- SSL certificate (e.g., Let's Encrypt)
- 3 monitoring agents (e.g., DataDog, UptimeRobot, Nagios)

## Diagram

![Diagram](secured_and_monitored_web_infrastructure.drawio.png)  

## Security Features

- **Firewalls**: Filter traffic to each component
- **HTTPS**: Encrypts user-server communication
- **SSL termination**: Done at the Load Balancer level

## Monitoring Features

- **Agents on each server**: Collect system and application metrics
- **Tools**: Examples: DataDog, New Relic, Uptime Robot
- **Collected data**: CPU usage, Memory, Disk, Request count (QPS), Error rates

## Risks and Limitations

| Issue | Explanation |
|-------|-------------|
| SSL at Load Balancer | Internal traffic is no longer encrypted |
| One MySQL writer | Write SPOF still exists |
| Same components per server | Redundant and inefficient for large-scale systems |
