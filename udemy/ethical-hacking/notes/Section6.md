# Introduction to Linux

## Exploring Kali Linux
* A bunch of pen testing tools are built in to the base image
* Tools are broken down into categories

## Navigating the File System
* Simple overview of `cd`, `pwd`, etc.

## Users and Priviliges
* `/etc/passwd` is a plain text-based database that contains information for all user accoutns
  * owned by root and has 644 permissions -> readable by anyone, only editable by root
  * See https://linuxize.com/post/etc-passwd-file/ for details
* `/etc/shadow` may allow you to crack passwords
  * Similar to `/etc/passwd`
  * Owned by root/shadow and ahs 640 permissions
* `su <user>` allows you to switch user

## Common Common Network commands
* `ifconfig` configure a network interface
* `iwconfig`  configure a wireless network interface
* `ping` send ICMP ECHO_REQUEST to network hosts
* `arp` associates IP addresses with MAC addresses
* `netstat`: Print network connections, routing tables, interface statistics, masquerade connections, and multicast memberships
* `route` show / manipulate the IP routing table

## Viewing, Creating, and Editing Files
* Overview of text editors, both in terminal and out of it

## Starting and Stopping Kali Services
* `service <name> start`
* Example: `service apache2 start`
  * Apache comes in kali linux by default
* `python -m SimpleHTTPServer` starts a webserver from the current directory
* Use `systemctl` to enable a service for all sessions

## Installing and Updating Tools
* Overview of `apt-get` and `git`

## Scripting with Bash
* Overview of `grep`, `cut`, `tr`, scripting, and `for` loops