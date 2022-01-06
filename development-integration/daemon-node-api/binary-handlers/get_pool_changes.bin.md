---
description: >-
  This method returns changes in pool containing unconfirmed transactions. Added
  transactions are returned as array of binary large objects (blobs)
---

# get\_pool\_changes.bin

### Input

| Argument    | Mandatory | Description                | Format |
| ----------- | --------- | -------------------------- | ------ |
| tailBlockId | yes       | Block hash of tail block   | Hash   |
| knownTxsIds | yes       | List of known block hashes | array  |

### Output

| Argument          | Description                                                  | Format |
| ----------------- | ------------------------------------------------------------ | ------ |
| isTailBlockActual | Is tailBlockId in pool                                       | bool   |
| addedTxs          | List of added transactions                                   | array  |
| deletedTxsIds     | List of transaction hashes of transactions no longer in pool | array  |
| status            | Status of request, "OK" if successful                        | string |
