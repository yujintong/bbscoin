# createDelayedTransaction

### Input

| Argument      | Mandatory | Description                               | Format |
| ------------- | --------- | ----------------------------------------- | ------ |
| addresses     | no        | List of source addresses                  | array  |
| transfers     | yes       | List of wallet RPC orders                 | array  |
| changeAddress | no        | Address to return unused amount in inputs | string |
| fee           | no        | Network fee                               | uint64 |
| anonymity     | no        | Anonymity level                           | uint32 |
| extra         | no        | Extra information for transaction         | string |
| paymentID     | no        | Payment ID for transaction                | string |
| unlockTime    | no        | Unlock time for transaction               | uint64 |

### Output

| Argument        | Description                                         | Format |
| --------------- | --------------------------------------------------- | ------ |
| transactionHash | Transaction hash of the created delayed transaction | string |
