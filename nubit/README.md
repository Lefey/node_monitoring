# nubit_zabbix
Zabbix monitoring template for monitoring Nubit node status.\
Install: Download zbx_nubit_template.yaml, import in to your zabbix instance, add host item, attach Nubit template to it and fill all macros values (select `Inherited and host macros` on host macros configuration tab)

Macros description:
| Macros | Default value | Mandatory | Description |
| --- | --- | --- | --- |
| `{$NODE_RPC_ADDRESS` | No | Yes | Nubit RPC node adress (http://ip:port or https URL) |
