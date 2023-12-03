# Linux Tools

| No. | Topic                                             |
| --- | ------------------------------------------------- |
| 1   | [System Information](#system-information)         |
| 2   | [System Monitoring](#system-monitoring)           |
| 3   | [Logging and Debugging](#logging-and-debugging)   |
| 4   | [File System Management](#file-system-management) |
| 5   | [Process Management](#process-management)         |
| 6   | [Network Management](#network-management)         |
| 7   | [User and Group Management](#user-and-group-management) |
| 8   | [Remote Access and Connectivity](#remote-access-and-connectivity) |


-----------------------------------------------------------------------------

## System Information <a name="system-information"></a>

These tools help users quickly gather essential information about the system, its configuration, and some resource utilization.

1. `uname` Retrieves basic system information like kernel name, version, and system architecture. 
2. `lsb_release` Provides Linux Standard Base information about the distribution.
3. `hostname` Shows the system's hostname.
4. `lscpu` Displays information about the CPU architecture.
5. `free` Offers details about system memory (RAM) usage.

## System Monitoring <a name="system-monitoring"></a>

Tools for observing and analyzing system performance, resource utilization, and other vital metrics.

1. `top` & `htop` & `btop` Provides real-time information about system processes. 
2. `vmstat` Reports virtual memory statistics.
3. `sar` Collects, reports, and saves system activity information.
4. `nmon` Provides performance monitoring and analysis.
5. `glances` Monitors system resources and processes in real-time.

## Logging and Debugging <a name="logging-and-debugging"></a>

This section covers tools and techniques for managing system logs, tracking events, and diagnosing issues. Commonly used tools here include `journalctl`, `dmesg`, `syslog`, `strace`, and `tcpdump`.

1. `journalctl`: Accesses and reads the systemd journal.
2. `dmesg`: Displays kernel-related messages.
3. `syslog`: Handles system log files.
4. `strace`: Traces system calls and signals.
5. `tcpdump`: Captures network packets.

## File System Management <a name="file-system-management"></a>

Tools dedicated to managing file systems, disk usage, and file permissions. Key utilities in this category are `df`, `du`, `mount`, `chown`, and `chmod`.

1. `df`: Displays disk space usage.
2. `du`: Shows disk space usage of files and directories.
3. `mount`: Mounts file systems.
4. `chown`: Changes file or group ownership.
5. `chmod`: Modifies file permissions.

## Process Management <a name="process-management"></a>

Focused on tools for controlling and monitoring processes on the system. Examples of tools in this category include `ps`, `pgrep`, `kill`, `htop`, and `systemctl`.

1. `ps`: Displays information about active processes.
2. `pgrep`: Searches for processes by name.
3. `kill`: Terminates processes.
4. `htop`: Interactive process viewer offering a better visualization of system processes.
5. `systemctl`: Controls systemd services.

## Network Management <a name="network-management"></a>

This section encompasses tools and utilities for managing network configurations, monitoring connectivity, and enhancing security. It includes tools like `iptables`, `ufw`, `ss`, `nmap`, and `fail2ban`.

1. **`iptables`**: Manages netfilter firewall rules.
2. `ufw`: Uncomplicated Firewall for managing iptables.
3. `ss`: Shows socket statistics.
4. `nmap`: Scans ports and discovers hosts on a network.
5. `fail2ban`: Intrusion prevention system that blocks malicious IP addresses.

## User and Group Management <a name="user-and-group-management"></a>

Tools for managing user accounts, groups, permissions, and access control. Commonly used tools here are `useradd`, `userdel`, `passwd`, `groupadd`, and `chown`.

1. `useradd`: Adds a new user account.
2. `userdel`: Deletes a user account.
3. `passwd`: Manages user passwords.
4. `groupadd`: Adds a new group.
5. `chown`: Changes file or group ownership.

## Remote Access and Connectivity <a name="remote-access-and-connectivity"></a>

This section focuses on tools enabling remote access, SSH configurations, and maintaining network connectivity. Tools like `ssh`, `scp`, `rsync`, `OpenVPN`, and `iptables` (for port forwarding) are included here.

1. `ssh`: Securely connects to a remote system.
2. `scp`: Securely copies files between systems.
3. `rsync`: Synchronizes files and directories between systems.
4. `OpenVPN`: Establishes secure connections over the internet.
5. `iptables`: Configures rules for network address translation (NAT) and port forwarding.

-------------- 
<!-- Backup -->
<!-- ## System Information <a name="system-information"></a>

### These tools help users quickly gather essential information about the system, its configuration, and some resource utilization.

- ### `uname`
  Retrieves basic system information like kernel name, version, and system architecture.
  > `uname >a`
- ### `lsb_release`
  Provides Linux Standard Base information about the distribution.
  > `lsb_release >a`
- ### `hostname`
  Shows the system's hostname.
  > `hostname`
- ### `lscpu`
  Displays information about the CPU architecture.
  > `lscpu`
- ### `free`
  Offers details about system memory (RAM) usage.
  > `free >h`


## System Monitoring <a name="system-monitoring"></a>

### Tools for observing and analyzing system performance, resource utilization, and other vital metrics.

- ### `top` & `htop` & `btop`
  Provides real-time information about system processes.
- ### `vmstat`
  Reports virtual memory statistics.
- ### `sar`
  Collects, reports, and saves system activity information.
- ### `nmon`
  Provides performance monitoring and analysis.
- ### `glances`
   Monitors system resources and processes in real-time.

## Logging and Debugging <a name="logging-and-debugging"></a>

This section covers tools and techniques for managing system logs, tracking events, and diagnosing issues. Commonly used tools here include:

- ### `journalctl`
  Accesses and reads the systemd journal.
    > `journalctl -u nginx.service`
- ### `dmesg`
  Displays kernel-related messages.
    > `dmesg | grep -i error`
- ### `syslog`
  Handles system log files.
    > `tail -f /var/log/syslog`
- ### `strace`
  Traces system calls and signals.
    > `strace -p PID`
- ### `tcpdump`
  Captures network packets.
    > `tcpdump -i eth0`

## File System Management <a name="file-system-management"></a>

Tools dedicated to managing file systems, disk usage, and file permissions. Key utilities in this category:

- ### `df`
  Displays disk space usage.
    > `df -h`
- ### `du`
  Shows disk space usage of files and directories.
    > `du -sh /path/to/directory`
- ### `mount`
  Mounts file systems.
    > `mount /dev/sdb1 /mnt`
- ### `chown`
  Changes file or group ownership.
    > `chown user:group file.txt`
- ### `chmod`
  Modifies file permissions.
    > `chmod 644 file.txt`

## Process Management <a name="process-management"></a>

Focused on tools for controlling and monitoring processes on the system. Examples of tools in this category include:

- ### `ps`
  Displays information about active processes.
    > `ps aux`
- ### `pgrep`
  Searches for processes by name.
    > `pgrep firefox`
- ### `kill`
  Terminates processes.
    > `kill PID`
- ### `htop`
  Interactive process viewer offering a better visualization of system processes.
    > `htop`
- ### `systemctl`
  Controls systemd services.
    > `systemctl start nginx`

## Network Management <a name="network-management"></a>

This section encompasses tools and utilities for managing network configurations, monitoring connectivity, and enhancing security. Includes tools like:

- ### `iptables`
  Manages netfilter firewall rules.
    > `iptables -A INPUT -p tcp --dport 80 -j ACCEPT`
- ### `ufw`
  Uncomplicated Firewall for managing iptables.
    > `ufw allow ssh`
- ### `ss`
  Shows socket statistics.
    > `ss -tulw`
- ### `nmap`
  Scans ports and discovers hosts on a network.
    > `nmap 192.168.1.1`
- ### `fail2ban`
  Intrusion prevention system that blocks malicious IP addresses.
    > `fail2ban-client status`

## User and Group Management <a name="user-and-group-management"></a>

Tools for managing user accounts, groups, permissions, and access control. Commonly used tools here are:

- ### `useradd`
  Adds a new user account.
    > `useradd -m newusername`
- ### `userdel`
  Deletes a user account.
    > `userdel existingusername`
- ### `passwd`
  Manages user passwords.
    > `passwd username`
- ### `groupadd`
  Adds a new group.
    > `groupadd newgroup`
- ### `chown`
  Changes file or group ownership.
    > `chown user:group file.txt`

## Remote Access and Connectivity <a name="remote-access-and-connectivity"></a>

This section focuses on tools enabling remote access, SSH configurations, and maintaining network connectivity. Tools like:

- ### `ssh`
  Securely connects to a remote system.
    > `ssh username@remote_host`
- ### `scp`
  Securely copies files between systems.
    > `scp /path/to/local/file username@remote_host:/path/to/destination`
- ### `rsync`
  Synchronizes files and directories between systems.
    > `rsync -avz /path/to/source username@remote_host:/path/to/destination`
- ### `OpenVPN`
  Establishes secure connections over the internet.
    > `openvpn client.ovpn`
- ### `iptables`
  Configures rules for network address translation (NAT) and port forwarding.
    > `iptables -A INPUT -p tcp --dport 80 -j ACCEPT` -->