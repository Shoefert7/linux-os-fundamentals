# linux-os-fundamentals
🐧 Linux Operating Systems Fundamentals & Administration

Course: CEIS 106 – Introduction to Operating Systems
Author: Shawn Hoefert
Date: May - June 2023
📌 Project Overview

This project provides a comprehensive exploration of Linux operating system fundamentals, focusing on essential command-line operations, system administration, and network configuration. It demonstrates practical skills in managing the Linux filesystem, creating and executing shell scripts, administering users and groups, configuring network interfaces, and monitoring system performance. This foundational knowledge is critical for cybersecurity professionals working with Linux-based servers and tools.
🎯 Key Objectives

    Linux Filesystem Mastery: Navigate, create, modify, and manage files and directories using command-line interface (CLI) commands.

    Shell Scripting: Develop, execute, and manage basic shell scripts for automation and task execution.

    User & Group Management: Administer user accounts and groups, including creation, modification, and removal, and understand associated permissions.

    Network Configuration: Discover, configure, and manage network interfaces and IP settings on a Linux system.

    System Monitoring: Monitor key system performance metrics, including processes, user activities, and network bandwidth usage.

    Command-Line Proficiency: Gain strong proficiency in essential Linux commands and utilities.

🔧 Tools & Technologies

    Operating System: Ubuntu Linux (CLI and GUI environments)

    Command-Line Utilities: pwd, cd, ls, mkdir, rm, cp, mv, locate, nano, chmod, useradd, groupadd, usermod, groupdel, userdel, tail, ipconfig, ping, dhclient, ifconfig, ps, top, htop, accton, lastcomm, nethogs (or similar network monitoring tools).

    Concepts: Filesystem Hierarchy Standard (FHS), Absolute vs. Relative Paths, File Permissions, PATH variable, Shell Scripting, User/Group IDs, DHCP, Network Interfaces, Process Management, System Accounting.

🔄 Workflow & Modules Summary

This project was structured around several key modules, each building practical Linux administration skills:

    Linux Filesystem Hierarchy & Management:

        Objective: Navigated the Linux filesystem tree, created, copied, moved, and removed directories and files.

        Skills: pwd, cd, ls, mkdir, rm, cp, mv, locate commands, understanding of file paths.

    Shell Scripting Fundamentals:

        Objective: Created and executed basic shell scripts, managed file permissions, and configured the PATH variable for script execution.

        Skills: Script creation (nano), chmod for permissions, echo, PATH variable management, understanding of redirection.

    User and Group Management:

        Objective: Administered user accounts and groups via both command-line (useradd, groupadd, usermod, groupdel, userdel) and graphical user interfaces. Tested user and group settings.

        Skills: User/Group Administration, Permissions, Security Best Practices for user accounts.

    Network Configuration:

        Objective: Discovered host IP configurations, managed network interfaces, and utilized network utilities.

        Skills: ipconfig, ping, dhclient, ifconfig commands, understanding of IP addresses, default gateways, DHCP, and DNS.

    System Performance Monitoring:

        Objective: Monitored Linux processes, user activities, and network bandwidth usage.

        Skills: Process management (ps, top, kill), user activity tracking (accton, lastcomm), network monitoring, understanding of system resource utilization.

💻 Command Examples & Outputs

Below are examples of commands executed and their outputs, demonstrating practical Linux skills:
Shell Script Creation & Execution

student@ubuntu1:~$: nano todolist
# (Content of todolist script, e.g., for a simple to-do list application)
student@ubuntu1:~$: chmod 755 todolist
student@ubuntu1:~$: ls -l todolist
-rwxr-xr-x 1 student student 199 May 16 22:51 todolist
student@ubuntu1:~$: ./todolist
Enter today's to-do-list (Press ENTER to complete):
1. work. 2. family. 3. school.
You entered: 1. work. 2. family. 3. school.

User and Group Creation (CLI)

# Example commands used for user/group management:
# sudo useradd -m newuser
# sudo groupadd newgroup
# sudo usermod -aG newgroup newuser
# cat /etc/group | grep students
# students:x:1002:student,mary

Network Interface Configuration

student@ubuntu1:~$: ifconfig eth0
# (Output showing network interface details, e.g., IP address, MAC address)
eth0: flags=4098<BROADCAST,MULTICAST> mtu 1500
        ether 00:15:5D:00:BA:04 txqueuelen 1000 (Ethernet)
        RX packets 6364  bytes 495436 (495.4 KB)
        RX errors 0  dropped 0  overruns 0  frame 0
        TX packets 10235 bytes 840393 (840.3 KB)
        TX errors 0  dropped 0  overruns 0  carrier 0  collisions 0

student@ubuntu1:~$: sudo ifconfig eth0 up
student@ubuntu1:~$: ifconfig eth0
eth0: flags=4163<UP,BROADCAST,RUNNING,MULTICAST> mtu 1500
        inet 192.168.1.107  netmask 255.255.255.0  broadcast 192.168.1.255
        inet6 fe80::7b9e:ebf5:11a6:34e4  prefixlen 64  scopeid 0x20<link>
        ether 00:15:5D:00:BA:04 txqueuelen 1000 (Ethernet)
# ... (additional output)

Network Connectivity Test

student@ubuntu1:/var/lib/dhcp$: ping -c 4 192.168.1.1
PING 192.168.1.1 (192.168.1.1) 56(84) bytes of data.
64 bytes from 192.168.1.1: icmp_seq=1 ttl=64 time=0.498 ms
# ... (ping results)
--- 192.168.1.1 ping statistics ---
4 packets transmitted, 4 received, 0% packet loss, time 3058ms
rtt min/avg/max/mdev = 0.323/0.500/0.647/0.116 ms

📈 Skills Demonstrated

    Linux System Administration: Proficient in managing Linux operating systems from the command line and GUI.

    Networking Fundamentals: Strong understanding of IP addressing, subnetting, and network interface management.

    Shell Scripting: Ability to automate tasks and manage system configurations using shell scripts.

    User & Access Management: Skilled in creating, modifying, and securing user and group accounts.

    System Monitoring: Capable of monitoring processes, user activity, and network traffic for operational awareness and security auditing.

    Problem-Solving & Troubleshooting: Diagnosing and resolving issues related to file permissions, network connectivity, and system processes.

    Command-Line Proficiency: Extensive experience with essential Linux commands for system interaction and data manipulation.
