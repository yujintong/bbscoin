---
description: Gets the balance of the wallet or an specific addresss.
---

# getbalance

#### Input

| Argument | Mandatory | Description             | Format |
| -------- | --------- | ----------------------- | ------ |
| address  | no        | Wallet address to query | string |

#### Output

| Argument         | Description                                      | Format |
| ---------------- | ------------------------------------------------ | ------ |
| availableBalance | Available balance that can be spent              | uint64 |
| lockedAmount     | Balance still locked in unconfirmed transactions | uint64 |

#### Usage

Replace "your\_password" and "TA4yACzMYuFYq7V6xVAWYHeS39jQ8w4mKRowpY6NskGuS1rZpjcWuCpdeCypwUCJrK9mGqVW9o1pY2EG3HW7BZkR2YRcc4YNa" in examples with real values from wallet daemon. Password is specified on command-line of wallet daemon, it is not returned by any API method for security reasons. You can get list of valid wallet addresses using getAddresses method.

```bash
curl -X POST http://ip_address:port/json_rpc -H 'Content-Type: application/json-rpc' -d '{"jsonrpc": "2.0", "method": "getBalance", "password": "your_password", "params": {}, "id": "1"}'
curl -X POST http://ip_address:port/json_rpc -H 'Content-Type: application/json-rpc' -d '{"jsonrpc": "2.0", "method": "getBalance", "password": "your_password", "params": {"address" : "TA4yACzMYuFYq7V6xVAWYHeS39jQ8w4mKRowpY6NskGuS1rZpjcWuCpdeCypwUCJrK9mGqVW9o1pY2EG3HW7BZkR2YRcc4YNa"}, "id": "1"}'
```
