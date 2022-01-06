---
description: >-
  This method clears all cached data and rescans the blockchain for
  transactions. If viewSecretKey is specified, old key will be discarded and
  rescan will use the new key for scanning transactions.
---

# reset

### Input

| Argument      | Mandatory | Description            | Format |
| ------------- | --------- | ---------------------- | ------ |
| viewSecretKey | no        | Secret view key to use | string |

### Output

| Argument | Description | Format |
| -------- | ----------- | ------ |
| none     |             |        |



### Usage

Replace "your\_password" and "viewSecretKey" in examples with real values from wallet daemon. Password is specified on command-line of wallet daemon, it is not returned by any API method for security reasons. Secret view key is returned by method getViewKey.

#### cURL

```bash
curl -X POST http://ip_address:port/json_rpc -H 'Content-Type: application/json-rpc' -d '{"jsonrpc": "2.0", "method": "reset", "password": "your_password", "params": {}, "id": "1"}'
curl -X POST http://ip_address:port/json_rpc -H 'Content-Type: application/json-rpc' -d '{"jsonrpc": "2.0", "method": "reset", "password": "your_password", "params": {"viewSecretKey" : "7968b4dd4114092ca71a90d38a542926bc32e0437bbc579e6de92ea4306ddf18"}, "id": "1"}'
```
