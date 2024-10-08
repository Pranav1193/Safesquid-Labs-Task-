Save the script to a file, e.g., 'monitor.sh'.
Make the script executable by running = chmod +x monitor.sh
Run the script without arguments to view the entire dashboard =./monitor.sh
Use command-line switches to view specific parts of the dashboard = ./monitor.sh -cpu -memory -network

# System Monitoring Dashboard
This script provides a real-time dashboard for monitoring various system resources on a proxy server. It supports monitoring CPU, memory, network activity, disk usage, system load, processes, and essential services.
## Usage
### Run the Full Dashboard
To run the full dashboard and monitor all resources, execute:
```bash
./monitor.sh

View Specific Resources
To monitor specific resources, use the following command-line switches:
-cpu : Top 10 applications by CPU and memory usage
-network : Network monitoring (connections, packet drops, MB in/out)
-disk : Disk usage by mounted partitions
-load : System load average and CPU breakdown
-memory : Memory and swap usage
-process : Number of active processes and top 5 processes
-services : Status of essential services (sshd, nginx/apache, iptables)
Example = ./monitor.sh -cpu -memory -network

Requirements
Bash
ps, ss or netstat, ifconfig or ip, df, uptime, mpstat, free, systemctl commands should be available on the system.
