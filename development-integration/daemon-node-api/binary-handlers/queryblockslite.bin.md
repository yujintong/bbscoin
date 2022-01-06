# queryblockslite.bin

### Input

| Argument   | Mandatory | Description          | Format |
| ---------- | --------- | -------------------- | ------ |
| block\_ids | yes       | List of block hashes | array  |
| timestamp  | yes       | Time stamp to start  | uint64 |

### Output

| Argument      | Description                               | Format |
| ------------- | ----------------------------------------- | ------ |
| status        | Status of the request, "OK" if successful | string |
| startHeight   | Start height                              | uint64 |
| currentHeight | Current height                            | uint64 |
| fullOffset    | Lowest block index                        | uint64 |
| items         | List of blocks                            | array  |
