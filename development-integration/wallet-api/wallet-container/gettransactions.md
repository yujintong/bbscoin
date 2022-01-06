---
description: Either blockHash or firstBlockIndex should be specified.
---

# getTransactions

### Input

| Argument        | Mandatory | Description                                    | Format |
| --------------- | --------- | ---------------------------------------------- | ------ |
| addresses       | no        | List of addresses to query transactions        | array  |
| blockHash       | no        | Block hash of first block                      | string |
| firstBlockIndex | no        | Index of first block                           | uint32 |
| blockCount      | yes       | Number of blocks to query                      | uint32 |
| paymentId       | no        | Payment ID to filter the returned transactions | string |

### Output

| Argument | Description    | Format |
| -------- | -------------- | ------ |
| items    | List of blocks | array  |
