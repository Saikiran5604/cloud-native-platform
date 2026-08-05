# Building a Container Without Docker

## Objective

Understand how Linux namespaces are combined to create container isolation.

## Commands

which unshare

sudo unshare --uts bash

sudo unshare --pid --fork bash

sudo unshare --uts --pid --mount --fork bash

## Observations

- A container starts as a Linux process.
- Namespaces isolate resources.
- Multiple namespaces together provide container-like isolation.
- Filesystem isolation is still missing.
