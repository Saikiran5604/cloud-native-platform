# Linux Namespaces

## Goal

Understand process isolation in Linux.

## Commands

which unshare
hostname
sudo unshare --uts bash
hostname container-demo
hostname
exit

## Observations

- Namespaces isolate operating system resources.
- UTS namespace isolates the hostname.
- Containers combine multiple namespaces.
