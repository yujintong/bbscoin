# estimateFusion

### Input

| Argument  | Mandatory | Description                                                                                                                                       | Format |
| --------- | --------- | ------------------------------------------------------------------------------------------------------------------------------------------------- | ------ |
| threshold | Yes       | Value that determines which outputs will be optimized. Only the outputs less than the threshold value will be included into a fusion transaction. | uint64 |
| addresses | No        | Array of strings, where each string is an address to take the funds from.                                                                         | array  |

### Output

| Argument         | Description                                                 | Format |
| ---------------- | ----------------------------------------------------------- | ------ |
| totalOutputCount | Total number of unspent outputs of the specified addresses. | uint64 |
| fusionReadyCount | Number of outputs that can be optimized.                    | uint64 |

### Usage

Replace "your\_password" and "TA4yACzMYuFYq7V6xVAWYHeS39jQ8w4mKRowpY6NskGuS1rZpjcWuCpdeCypwUCJrK9mGqVW9o1pY2EG3HW7BZkR2YRcc4YNa" in examples with real values from wallet daemon. Password is specified on command-line of wallet daemon, it is not returned by any API method for security reasons. You can get list of valid wallet addresses using getAddresses method.

#### cURL

```bash
curl -X POST http://ip_address:port/json_rpc -H 'Content-Type: application/json-rpc' -d '{"jsonrpc": "2.0", "method": "estimateFusion", "password": "your_password", "params": {"addresses": ["TA4yACzMYuFYq7V6xVAWYHeS39jQ8w4mKRowpY6NskGuS1rZpjcWuCpdeCypwUCJrK9mGqVW9o1pY2EG3HW7BZkR2YRcc4YNa"], "threshold" : 100000000}, "id": "1"}'
```
