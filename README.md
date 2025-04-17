# Netdata Monitoring Setup

## Objective
This project aims to install Netdata, a free and open-source monitoring tool, to visualize system and application performance metrics.

## Tools
- **Netdata**: Open-source monitoring tool
- **Docker**: Containerization platform

## Installation Guide

### Prerequisites
- Ensure that Docker is installed and running on your system. Download Docker from [here](https://www.docker.com/get-started).

### Step 1: Run Netdata via Docker
Open the terminal and execute the following command to run Netdata in a Docker container:

```bash
docker run -d --name=netdata -p 19999:19999 netdata/netdata
```

### Step 2: Access the Dashboard
Once the container which is running, open the web browser and navigate to:

```
http://localhost:19999
```

### Step 3: Monitor System Resources
In the Netdata dashboard, we can monitor various metrics, including:
- **CPU Usage**
- **Memory Usage**
- **Disk I/O**
- **Docker Containers** (if applicable)

### Step 4: Explore Alerts and Chart Panels
The dashboard provides alerts and various chart panels for detailed insights into system performance.

### Step 5: Check Logs
We can explore logs located in `/var/log/netdata` for any issues or detailed logging information.

## Troubleshooting
If encountered connection issues, consider the following:

- **Check if the Netdata container is running**:
  ```bash
  docker ps
  ```

- **Restart the container if necessary**:
  ```bash
  docker start netdata
  ```

- **Ensure Docker is installed and running properly**.

## Deliverables
- **Screenshot of the Dashboard**:

- **Running Metrics**: Note down key metrics which is being monitored, such as CPU load, memory usage, and disk activity.

## Conclusion
By following this guide, I was able to successfully install and monitor system resources using Netdata.