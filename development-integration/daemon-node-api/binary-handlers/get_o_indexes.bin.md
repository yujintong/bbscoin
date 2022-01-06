---
description: This method returns global outputs indexes of a transaction.
---

# get\_o\_indexes.bin

### Input

| Argument | Mandatory | Description      | Format |
| -------- | --------- | ---------------- | ------ |
| txid     | yes       | Transaction hash | Hash   |

### Output

| Argument   | Description                               | Format |
| ---------- | ----------------------------------------- | ------ |
| o\_indexes | List of outputs indexes                   | array  |
| status     | Status of the request, "OK" if successful | string |
