# rspamd_config

Copy `local.d/nforcer/_multimap_nforcer.conf` to your rspamd config directory 
`/etc/rspamd/local.d/_multimap_nforcer.conf`
and restart rspamd to enable the nforcer multimap rules.

Enable by adding this to your /etc/rspamd/local.d/multimap.conf file:

```text
.include(try=true,priority=1,duplicate=merge) "$LOCAL_CONFDIR/local.d/_multimap_nforcer.conf"

```

