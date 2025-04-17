# 📊 DevOps Task 7 - System Monitoring with Netdata

## 📌 Objective
Deploy Netdata using Docker to monitor real-time system performance metrics like CPU, memory, disk, and Docker containers.

## 🛠️ Tools Used
- Docker
- Netdata (open-source monitoring)

## 🚀 Setup Instructions

### Step 1: Run Netdata with Docker

```bash
docker run -d --name=netdata -p 19999:19999 --cap-add=SYS_PTRACE -v netdataconfig:/etc/netdata -v netdatalib:/var/lib/netdata -v netdatacache:/var/cache/netdata -v /etc/passwd:/host/etc/passwd:ro -v /etc/group:/host/etc/group:ro -v /proc:/host/proc:ro -v /sys:/host/sys:ro -v /etc/os-release:/host/etc/os-release:ro netdata/netdata

### **Step 2: Monitored Metrics**

In this task, I successfully monitored the following system metrics using Netdata:

- ✅ **CPU Usage**
- ✅ **Memory Usage**
- ✅ **Disk I/O**
- ✅ **Docker Containers**
- ✅ **Container Logs** (`/var/log/netdata`)

### **Step 3: 📸 Screenshots**

Here are the screenshots showcasing the system metrics:

- CPU usage

- Memory stats

- Disk usage

- Docker container metrics

- Logs and charts

