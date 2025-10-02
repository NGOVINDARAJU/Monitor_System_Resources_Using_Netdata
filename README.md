# Monitor System Resources Using Netdata (Windows + Docker)

## Objective
Install Netdata in Docker and visualize system performance metrics.

## Steps I Followed
1. Removed old container:
   ```bash
   docker rm -f netdata
2. Started Netdata:
   ```bash
   docker run -d --name=netdata -p 19999:19999 --restart unless-stopped netdata/netdata
3. Checked container:
   ```bash
   docker ps
4.Opened dashboard at http://localhost:19999
## Metrics Observed
- CPU: Shows usage spikes when running tasks.
- Memory: Shows free vs used RAM.
- Disk: Displays read/write operations.
- Network: Shows incoming/outgoing traffic.
- Alarms: Highlights any warnings.
## Deliverables
- Screenshots of CPU, Memory, Disk, Alarms.
- docker-ps.txt → Running containers list.
- netdata-logs.txt → Container logs.
  
