# sendTransaction

### Input

| Argument      | Mandatory | Description                               | Format |
| ------------- | --------- | ----------------------------------------- | ------ |
| addresses     | no        | List of addresses to send the orders from | array  |
| transfers     | yes       | List of wallet RPC orders                 | array  |
| changeAddress | no        | Address to send unused amount of inputs   | string |
| fee           | no        | Network fee                               | uint64 |
| anonymity     | no        | Anonymity level                           | uint32 |
| extra         | no        | Extra information for transaction         | string |
| paymentId     | no        | Payment ID for transaction                | string |
| unlockTime    | no        | Unlock time for transaction               | uint64 |

### Output

| Argument        | Description                              | Format |
| --------------- | ---------------------------------------- | ------ |
| transactionHash | Transaction hash of the sent transaction | string |

### Usage

Replace "your\_password" and "TA4yACzMYuFYq7V6xVAWYHeS39jQ8w4mKRowpY6NskGuS1rZpjcWuCpdeCypwUCJrK9mGqVW9o1pY2EG3HW7BZkR2YRcc4YNa" in examples with real values from wallet daemon. Password is specified on command-line of wallet daemon, it is not returned by any API method for security reasons. You can get list of valid wallet addresses using getAddresses method.

Replace "TA4hZYd77tqhHnjXxmq7GvZpPZSSx8CthWy9ZufqF8kjZBBN1WAg38uGLihKnLUKTgHC7qSoM5yWneVsyCdkrL6L1mgAuuuM2" with the wallet address of the recipient.

`amount` and `fee` fields are in atomic units.

You can add multiple recipients separated with comma, each enclosed between `{` and `}`.

You only need to specify `changeAddress` if you use multiple addresses to send the funds or if `addresses` list is empty and wallet file contains multiple addresses.

#### cURL

```bash
curl -X POST http://ip_address:port/json_rpc -H 'Content-Type: application/json-rpc' -d '{"jsonrpc": "2.0", "method": "sendTransaction", "password": "your_password", "params": {"anonymity": 0, "addresses": ["TA4yACzMYuFYq7V6xVAWYHeS39jQ8w4mKRowpY6NskGuS1rZpjcWuCpdeCypwUCJrK9mGqVW9o1pY2EG3HW7BZkR2YRcc4YNa"], "transfers": [{"address": "TA4hZYd77tqhHnjXxmq7GvZpPZSSx8CthWy9ZufqF8kjZBBN1WAg38uGLihKnLUKTgHC7qSoM5yWneVsyCdkrL6L1mgAuuuM2", "amount": 100}], "fee": 1}, "id": "1"}'
```
