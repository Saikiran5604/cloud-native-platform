# Linux cgroups

## Goal

Understand Linux resource control.

## Commands

stat -fc %T /sys/fs/cgroup

ls /sys/fs/cgroup

cat /sys/fs/cgroup/memory.current

cat /sys/fs/cgroup/memory.max

cat /sys/fs/cgroup/cpu.max

## Observations

- cgroups limit resources.
- Docker uses cgroups.
- Kubernetes resource limits are enforced through cgroups.
