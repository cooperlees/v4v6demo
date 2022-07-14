# IPv4 via IPv6 Linux netns Demo

A simple Linux network namespace demo of IPv4 via IPv6 next hops on a point to point link.

## Lab topology

TBA

## Requirements

- Linux >= 5.2 (kernel)
- iproute / `ip` command to drive netlink
- python >= 3.8
  - Unless you want to configure the netns yourself

## Create netns

### Install json2netns

- `python3 -m venv /tmp/j [--upgrade-deps]`
- `/tmp/j/bin/pip install json2netns`

### Create the network namespaces with json2netns

- `/tmp/j/bin/json2netns create p2p_json2netns.json`
- Lets check the netns
  - `/tmp/j/bin/json2netns check`

## Lab Time

- TBA

## Delete netns

This will delete the two netns's

- `/tmp/j/bin/json2netns delete p2p_json2netns.json`
