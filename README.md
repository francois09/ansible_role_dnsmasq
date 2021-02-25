DNSMASQ Ansible role
====================

Role to manage DNSMASQ in the specific case of using it as a DNS (tcp/udp) proxy.

It creates a "fake" /etc/resolv.conf like file filled with local DNS (members of the `nameserver` group in inventory)

Requirements
------------

No requirements

Role Variables
--------------

* `dnsmasq__install` For install only (default: False)
* `dnsmasq__configure` For configuration  (default: False)

* `dnsmasq__default_packages` Packages needed
* `dnsmasq__conf_file` config file (Default: "/etc/dnsmasq.proxy.conf")
* `dnsmasq__resolv_conf_file` Use resolv.conf specific file (Default : "/etc/resolv.conf.dnsmasq")
* `dnsmasq__pid_file` PID file (Default : "/var/run/proxy.dnsmasq.pid")

* `dnsmasq__neg_ttl` Negative (fail) TTL (Default : 5)

Dependencies
------------

None

Example Playbooks
-----------------


License
-------

GPL v3

Author Information
------------------

François TOURDE