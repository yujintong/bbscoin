# sendFusionTransaction

### Input

| Argument           | Mandatory | Description                                         | Format |
| ------------------ | --------- | --------------------------------------------------- | ------ |
| threshold          | yes       | Target threshold for optimized outputs              | uint64 |
| anonymity          | no        | Anonymity level of fusion transaction               | uint32 |
| addresses          | yes       | Source addresses to be optimized                    | array  |
| destinationAddress | yes       | Destination address for receiving optimized outputs | string |

### Output

| Argument        | Description                                        | Format |
| --------------- | -------------------------------------------------- | ------ |
| transactionHash | Transaction hash of the created fusion transaction | string |

### Usage

Replace "your\_password" and "TA4yACzMYuFYq7V6xVAWYHeS39jQ8w4mKRowpY6NskGuS1rZpjcWuCpdeCypwUCJrK9mGqVW9o1pY2EG3HW7BZkR2YRcc4YNa" in examples with real values from wallet daemon. Password is specified on command-line of wallet daemon, it is not returned by any API method for security reasons. You can get list of valid wallet addresses using getAddresses method.

#### cURL

```bash
curl -X POST http://ip_address:port/json_rpc -H 'Content-Type: application/json-rpc' -d '{"jsonrpc": "2.0", "method": "sendFusionTransaction", "password": "your_password", "params": {"addresses": ["TA4yACzMYuFYq7V6xVAWYHeS39jQ8w4mKRowpY6NskGuS1rZpjcWuCpdeCypwUCJrK9mGqVW9o1pY2EG3HW7BZkR2YRcc4YNa"], "destinationAddress": "TA4yACzMYuFYq7V6xVAWYHeS39jQ8w4mKRowpY6NskGuS1rZpjcWuCpdeCypwUCJrK9mGqVW9o1pY2EG3HW7BZkR2YRcc4YNa", "threshold" : 100000000, "anonymity": 0}, "id": "1"}'
```
