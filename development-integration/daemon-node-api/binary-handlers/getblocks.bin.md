# getblocks.bin

### Input

| Argument   | Mandatory | Description    | Format |
| ---------- | --------- | -------------- | ------ |
| block\_ids | yes       | List of hashes | array  |

### Output

| Argument        | Description                               | Format |
| --------------- | ----------------------------------------- | ------ |
| blocks          | List of raw blocks                        | array  |
| start\_height   | Start height                              | uint64 |
| current\_height | Total number of blocks                    | uint64 |
| status          | Status of the request, "OK" if successful | string |
