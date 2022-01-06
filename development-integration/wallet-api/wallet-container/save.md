---
description: >-
  This method saves the current wallet container to disk using same filename as
  when loaded.
---

# save

### Input

| Argument | Mandatory | Description | Format |
| -------- | --------- | ----------- | ------ |
| none     |           |             |        |

### Output

| Argument | Description | Format |
| -------- | ----------- | ------ |
| none     |             |        |

### Usage

Replace "your_password", "ip\_address_", "port" in example with real value from wallet daemon. Password is specified on command-line of wallet daemon, it is not returned by any API method for security reasons.

#### cURL

```bash
curl -X POST http://ip_address:port/json_rpc -H 'Content-Type: application/json-rpc' -d '{"jsonrpc": "2.0", "method": "save", "password": "your_password", "params": {}, "id": "1"}'
```
