# autonity_zabbix
Zabbix monitoring template for monitoring autonity node and validator status.\
Install: Download zbx_autonity_template.yaml, import in to your zabbix instance, add host item, attach Autonity template to it and fill all macros values (select `Inherited and host macros` on host macros configuration tab)

Macros description:
| Macros | Default value | Mandatory | Description |
| --- | --- | --- | --- |
| `{$VALIDATOR_ADDRESS}` | Empty | Yes | Autonity validator adress, for example 0xc495ceff1e17d942c633c32e5f4d74efbb844028 |
| `{$AUTONITY_RPC}` | https://rpc1.piccadilly.autonity.org | Yes | Autonity RPC node adress, you can use your own node here |
