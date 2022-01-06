---
description: >-
  This method saves/stores the current wallet container to disk using same
  filename as when loaded.
---

# store

#### Input

| Argument | Mandatory | Description | Format |
| -------- | --------- | ----------- | ------ |
| none     |           |             |        |

#### Output

| Argument | Description | Format |
| -------- | ----------- | ------ |
| none     |             |        |

#### Usage

Replace "your\_password" in example with real value from wallet daemon. Password is specified on command-line of wallet daemon, it is not returned by any API method for security reasons.

```bash
# With a password
curl -X POST http://ip_address:port/json_rpc -H 'Content-Type: application/json-rpc' -d '{"jsonrpc": "2.0", "method": "store", "password": "your_password", "params": {}, "id": "1"}'

# Without a password
curl -X POST http://ip_address:port/json_rpc -H 'Content-Type: application/json-rpc' -d '{"jsonrpc": "2.0", "method": "store", "password": "your_password", "params": {}, "id": "1"}'
```
