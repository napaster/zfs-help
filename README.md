## zfs-help
Role for the help https://github.com/zabbix/community-templates/tree/main/Operating_Systems/Linux/template_zfs_on_linux/7.0

To use the Zabbix ZFS on Linux template, you must first install a correctly configured userparams file on any machines running the zabbix agent and using ZFS.
Additionally, for monitoring of scrub and resilver stats you must install the ZED integration script.

## Requirements

* Ansible 2.5+;

## Extra

The role support array of options for `zfs[].settings`. Options is not
validate and pass as-is. For all possible options please consult with

## Example configuration

```yaml
---
zfs:
# Enable deploy or not (default is 'false').
  - setings: 'true'
    enabled: 'true'
    restart: 'true'