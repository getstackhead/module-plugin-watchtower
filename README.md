# StackHead: Watchtower module

StackHead module for Watchtower.

## Installation

Install it via `ansible-galaxy`:

```
ansible-galaxy install getstackhead.stackhead_plugin_watchtower
```

In order to use Watchtower with [StackHead](https://get.stackhead.io), add it to `stackhead__plugins` in your inventory file:

```yaml
# inventory for integration test
---
all:
  vars:
    stackhead__plugins:
      - getstackhead.stackhead_plugin_watchtower
  hosts:
    myserver:
      ansible_host: 123.456.789 # ...
      stackhead:
        applications:
          # ...
```
