# cosmos_zabbix
Zabbix monitoring template for monitoring Cosmos SDK node and validator status.\
Install: Download zbx_cosmos_template.yaml, import in to your zabbix instance, add host item, attach Cosmos template to it and fill all macros values (select `Inherited and host macros` on host macros configuration tab)

Macros description:
| Macros | Default value | Mandatory | Description |
| --- | --- | --- | --- |
| `{$NODE_RPC_ADDRESS}` | Empty | Yes | Node RPC address (http://ip:port or https URL) example: http://1.2.3.4:26657 |
| `{$NODE_API_ADDRESS}` | Empty | Yes for validator monitoring | Node API address (http://ip:port or https URL) example: http://1.2.3.4:1317, it is recommended to use any public endpoint |
| `{$VALOPER}` | Empty | Yes for validator monitoring | Validator operator address, can be obtained using command `<binary_name> keys show <wallet_name> --bech val -a` |
| `{$VALCONS}` | Empty | Yes for validator monitoring | Validator consensus address, can be obtained using command `<binary_name> tendermint show-address` |
| `{$SELF_BOND_WALLET}` | Empty | Yes for wallet monitoring | Self bond wallet address |
| `{$DENOM}` | 1.0E-6 | Yes to show validator comission and staking rewards | Denomination multiplier, example: 1.0E-6 (equal to 0.000001) |
| `{$DENOM_TICKER}` | Empty | Yes to show validator comission and staking rewards | Denom ticker, example: uatom, can be obtained using the command  `<binary_name> q staking params`|
