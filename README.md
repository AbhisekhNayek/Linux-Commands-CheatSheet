# Linux Command Cheat Sheet

A comprehensive cheat sheet for Linux commands, from basic to advanced.

## Table of Contents

1. [Introduction](#introduction)
2. [Basic Commands](#basic-commands)
3. [File and Directory Management](#file-and-directory-management)
4. [Text Manipulation](#text-manipulation)
5. [Process Management](#process-management)
6. [System Information](#system-information)
7. [User and Group Management](#user-and-group-management)
8. [Network Commands](#network-commands)
9. [Package Management](#package-management)
10. [Advanced Commands](#advanced-commands)

## Introduction

Welcome to the Linux Command Cheat Sheet! This repository contains a collection of Linux commands and their descriptions, ranging from basic operations to advanced system management.

## Basic Commands

### 1. `pwd`

Print the current working directory.

```bash
$ pwd
```

### 2. `ls`

List files and directories in the current directory.

```bash
$ ls
$ ls -l
$ ls -a
$ ls -lh
$ ls -R
```

### 3. `cd`

Change the current directory.

```bash
$ cd directory_name
$ cd ..
$ cd -
```

### 4. `mkdir`

Create a new directory.

```bash
$ mkdir directory_name
$ mkdir -p path/to/directory
```

### 5. `rm`

Remove files or directories.

```bash
$ rm file_name
$ rm -r directory_name
$ rm -f file_name
$ rm -i file_name
```

## File and Directory Management

### 1. `cp`

Copy files or directories.

```bash
$ cp file1 file2
$ cp -r dir1 dir2
$ cp -u file1 file2
```

### 2. `mv`

Move or rename files and directories.

```bash
$ mv file1 file2
$ mv oldname newname
$ mv file1 dir/
```

### 3. `ln`

Create hard or symbolic links.

```bash
$ ln -s target link_name
$ ln file link
```

### 4. `chmod`

Change file permissions.

```bash
$ chmod permissions file
$ chmod -R permissions directory
```

### 5. `chown`

Change file owner and group.

```bash
$ chown owner:group file
$ chown -R owner:group directory
```

## Text Manipulation

### 1. `cat`

Display the contents of a file.

```bash
$ cat filename
$ cat file1 file2 > newfile
```

### 2. `grep`

Search for a pattern in a file.

```bash
$ grep pattern filename
$ grep -r pattern directory
```

### 3. `sed`

Stream editor for text transformation.

```bash
$ sed 's/old/new/g' filename
```

### 4. `awk`

Pattern scanning and processing language.

```bash
$ awk '{print $1}' filename
```

### 5. `sort`

Sort lines of text files.

```bash
$ sort filename
$ sort -r filename
```

## Process Management

### 1. `ps`

Display information about active processes.

```bash
$ ps
$ ps aux
$ ps -ef
```

### 2. `kill`

Terminate a process.

```bash
$ kill process_id
$ kill -9 process_id
```

### 3. `top`

Display and update sorted information about processes.

```bash
$ top
```

### 4. `nice`

Run a command with a modified scheduling priority.

```bash
$ nice -n value command
```

## System Information

### 1. `uname`

Display system information.

```bash
$ uname -a
$ uname -r
```

### 2. `df`

Display disk space usage.

```bash
$ df -h
$ df -i
```

### 3. `free`

Display amount of free and used memory.

```bash
$ free -h
```

## User and Group Management

### 1. `useradd`

Add a new user.

```bash
$ sudo useradd username
$ sudo passwd username
```

### 2. `usermod`

Modify user properties.

```bash
$ sudo usermod -aG groupname username
```

### 3. `passwd`

Change user password.

```bash
$ passwd username
```

### 4. `groupadd`

Add a new group.

```bash
$ sudo groupadd groupname
```

### 5. `id`

Display user and group information.

```bash
$ id username
```

## Network Commands

### 1. `ifconfig`

Display network interface information.

```bash
$ ifconfig
$ ifconfig -a
```

### 2. `ping`

Check network connectivity.

```bash
$ ping example.com
$ ping -c count example.com
```

### 3. `traceroute`

Trace the route to a network host.

```bash
$ traceroute example.com
```

### 4. `netstat`

Display network connections.

```bash
$ netstat -tuln
```

## Package Management

### 1. `apt-get`

Install, update, or remove packages on Debian-based systems.

```bash
$ sudo apt-get install package_name
$ sudo apt-get update
$ sudo apt-get remove package_name
```

### 2. `yum`

Install, update, or remove packages on Red Hat-based systems.

```bash
$ sudo yum install package_name
$ sudo yum update
$ sudo yum remove package_name
```

### 3. `dpkg`

Debian package management.

```bash
$ dpkg -i package.deb
$ dpkg -l
```

## Advanced Commands

### 1. `find`

Search for files in a directory hierarchy.

```bash
$ find /path/to/search -name filename
$ find /path -type f -mtime -5
```

### 2. `tar`

Create or extract tar archives.

```bash
$ tar -cvf archive.tar files
$ tar -xvf archive.tar
$ tar -czvf archive.tar.gz files
```

### 3. `curl`

Transfer data from or to a server.

```bash
$ curl -O http://example.com/file
$ curl -u user:password -X POST -d "data" http://example.com/api
```

### 4. `wget`

Download files from the internet.

```bash
$ wget http://example.com/file
```

### 5. `ssh`

Secure Shell for remote login.

```bash
$ ssh user@hostname
```

## Contributing

Feel free to contribute by adding new commands or improving existing ones. See [CONTRIBUTING.md](CONTRIBUTING.md) for more information.

## License

This project is licensed under the [MIT License](LICENSE).
