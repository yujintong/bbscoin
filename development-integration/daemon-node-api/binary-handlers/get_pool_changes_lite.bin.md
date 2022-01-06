# get\_pool\_changes\_lite.bin

### Input

| Argument    | Mandatory | Description                      | Format |
| ----------- | --------- | -------------------------------- | ------ |
| tailBlockId | yes       | Block hash of tail block         | Hash   |
| knownTxsIds | yes       | List of known transaction hashes | array  |

### Output

| Argument          | Description                                        | Format |
| ----------------- | -------------------------------------------------- | ------ |
| isTailBlockActual | Is tailBlockId in pool                             | bool   |
| addedTxs          | List of transaction prefixes of added transactions | array  |
| deletedTxsIds     | List of transaction hashes of deleted transactions | array  |
| status            | Status of the request, "OK" if successful          | string |
