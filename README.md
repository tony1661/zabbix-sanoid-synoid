# zabbix-sanoid-synoid
Monitoring template for Sanoid and Syncoid via Zabbix

This can be used for monitoring your Sanoid setup using the sanoid included `--monitor-*` commands.

This can also be used to monitor your replicated ZFS datasets via Syncoid.

The `--monitor-*` commands look at the sanoid.conf file so if you are monitoring a server that has it's ZFS datasets replicated via Syncoid, you will need the sanoid.conf file to be present so that it knows what your replication expextations are.

### How to use this
 - Copy the `sanoid.conf` file to 
    - `/etc/zabbix/zabbix_agent2.d/plugins.d` (is using Agent 2)
    - `/etc/zabbix/zabbix_agentd.d/` (if using Agent 1)

 - Import the zabbix template yaml file
 - Add the template to your host