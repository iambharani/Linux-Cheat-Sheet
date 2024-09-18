# linux-cheat-sheet
Here's a comprehensive Linux cheat sheet with a table of contents that you can use for a GitHub README. This cheat sheet covers basic commands and concepts commonly used in Linux environments.

---

# Linux Cheat Sheet

A handy reference for common Linux commands and concepts.

## Table of Contents

1. [File and Directory Operations](#file-and-directory-operations)
2. [File Permissions](#file-permissions)
3. [Process Management](#process-management)
4. [Package Management](#package-management)
5. [Network Commands](#network-commands)
6. [Disk Usage and Management](#disk-usage-and-management)
7. [System Information](#system-information)
8. [Text Processing](#text-processing)
9. [Search Commands](#search-commands)
10. [User and Group Management](#user-and-group-management)
11. [Archiving and Compression](#archiving-and-compression)
12. [System Monitoring](#system-monitoring)
13. [Remote Access](#remote-access)
14. [Miscellaneous Commands](#miscellaneous-commands)

---

## File and Directory Operations

- **List files and directories**
  ```bash
  ls
  ls -l       # Detailed listing
  ls -a       # Show hidden files
  ```

- **Change directory**
  ```bash
  cd [directory]
  cd ..       # Move up one directory
  ```

- **Print working directory**
  ```bash
  pwd
  ```

- **Create directory**
  ```bash
  mkdir [directory]
  ```

- **Remove directory**
  ```bash
  rmdir [directory]        # Empty directory
  rm -r [directory]        # Directory with files
  ```

- **Copy files and directories**
  ```bash
  cp [source] [destination]
  cp -r [source] [destination]  # Recursive copy
  ```

- **Move or rename files and directories**
  ```bash
  mv [source] [destination]
  ```

- **Remove files**
  ```bash
  rm [file]
  ```

## File Permissions

- **Change file permissions**
  ```bash
  chmod [permissions] [file]
  chmod +x [file]       # Add execute permission
  chmod 755 [file]      # Set permissions to rwxr-xr-x
  ```

- **Change file owner**
  ```bash
  chown [owner] [file]
  ```

- **Change file group**
  ```bash
  chgrp [group] [file]
  ```

## Process Management

- **List processes**
  ```bash
  ps
  ps aux           # Detailed listing
  ```

- **Kill process**
  ```bash
  kill [pid]
  kill -9 [pid]    # Force kill
  ```

- **Find process**
  ```bash
  pgrep [name]
  ```

- **View running processes interactively**
  ```bash
  top
  ```

## Package Management

- **Debian-based (e.g., Ubuntu)**
  ```bash
  sudo apt update
  sudo apt upgrade
  sudo apt install [package]
  sudo apt remove [package]
  ```

- **Red Hat-based (e.g., CentOS)**
  ```bash
  sudo yum update
  sudo yum install [package]
  sudo yum remove [package]
  ```

- **Check package information**
  ```bash
  dpkg -l [package]       # Debian-based
  rpm -q [package]        # Red Hat-based
  ```

## Network Commands

- **Check network status**
  ```bash
  ifconfig
  ip a
  ```

- **Ping a host**
  ```bash
  ping [host]
  ```

- **Download files**
  ```bash
  wget [url]
  curl -O [url]
  ```

- **Check open ports**
  ```bash
  netstat -tuln
  ```

## Disk Usage and Management

- **Check disk usage**
  ```bash
  df -h
  ```

- **Check directory size**
  ```bash
  du -sh [directory]
  ```

- **Mount and unmount filesystems**
  ```bash
  mount [device] [mount_point]
  umount [mount_point]
  ```

## System Information

- **Check system information**
  ```bash
  uname -a
  lsb_release -a
  ```

- **Check memory usage**
  ```bash
  free -h
  ```

- **Check CPU information**
  ```bash
  lscpu
  ```

## Text Processing

- **View file contents**
  ```bash
  cat [file]
  less [file]
  more [file]
  ```

- **Find and replace text**
  ```bash
  sed 's/[search]/[replace]/' [file]
  ```

- **Search for text**
  ```bash
  grep [search_term] [file]
  ```

## Search Commands

- **Find files**
  ```bash
  find [directory] -name [filename]
  ```

- **Locate files**
  ```bash
  locate [filename]
  ```

## User and Group Management

- **Add a user**
  ```bash
  sudo adduser [username]
  ```

- **Delete a user**
  ```bash
  sudo deluser [username]
  ```

- **Add a group**
  ```bash
  sudo addgroup [groupname]
  ```

- **Add user to a group**
  ```bash
  sudo usermod -aG [groupname] [username]
  ```

## Archiving and Compression

- **Create a tar archive**
  ```bash
  tar -cvf [archive.tar] [files]
  ```

- **Extract a tar archive**
  ```bash
  tar -xvf [archive.tar]
  ```

- **Compress with gzip**
  ```bash
  gzip [file]
  ```

- **Extract gzip**
  ```bash
  gunzip [file.gz]
  ```

## System Monitoring

- **Monitor system performance**
  ```bash
  top
  htop
  ```

- **Check disk I/O**
  ```bash
  iostat
  ```

## Remote Access

- **SSH into a server**
  ```bash
  ssh [user]@[host]
  ```

- **Transfer files with SCP**
  ```bash
  scp [source] [user]@[host]:[destination]
  ```

## Miscellaneous Commands

- **Show calendar**
  ```bash
  cal
  ```

- **Show date**
  ```bash
  date
  ```

- **Show current directory**
  ```bash
  pwd
  ```

---

Feel free to customize this cheat sheet according to your needs or add more details about each command.
