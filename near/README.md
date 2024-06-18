# near_zabbix
Zabbix monitoring template for monitoring Near node and validator status.\
Install: Download zbx_near_template.yaml, import in to your zabbix instance, add host item, attach Near template to it and fill all macros values (select `Inherited and host macros` on host macros configuration tab)

Macros description:
| Macros | Default value | Mandatory | Description |
| --- | --- | --- | --- |
| `{$VALIDATOR_POOL}` | Empty | Yes | Near validator stake pool adress, for example myvalidator.pool.near |
| `{$NODE_RPC_ADDRESS}` | Empty | Yes | Near RPC node adress (http://ip:port or https URL), you can use your own node here |

<picture> <img align="left" src="https://github.com/Lefey/Lefey/raw/main/img/stakewars_dashboard.jpg"></picture>
