prometheus
==========

This playbook is used to install prometheus automatically.

Role Variables
--------------

```yaml
prometheus_version: PROMETHEUS_VERSION
prometheus_base_dir: PROMETHEUS_BASE_DIR (default: /opt/prometheus)
prometheus_listen_address: PROMETHEUS_LISTEN_ADDRESS (default: 0.0.0.0)
prometheus_listen_port: PROMETHEUS_LISTEN_PORT (default: 9090)
```

Dependencies
------------

- pylabs.sysbase

Example Playbook
----------------

```yaml
- hosts: servers
  roles:
    - role: pylabs.prometheus
  vars:
    prometheus_version: "2.21.0"
```

License
-------

MIT

Author Information
------------------

William Wu <william@pylabs.org>
