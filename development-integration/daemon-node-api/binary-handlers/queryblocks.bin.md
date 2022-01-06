# queryblocks.bin

### Input

| Argument   | Mandatory | Description         | Format |
| ---------- | --------- | ------------------- | ------ |
| block\_ids | yes       | List of hashes      | array  |
| timestamp  | yes       | Time stamp to start | uint64 |

### Output

| Argument        | Description                               | Format |
| --------------- | ----------------------------------------- | ------ |
| status          | Status of the request, "OK" if successful | string |
| start\_height   | Starting height                           | uint64 |
| current\_height | Current height                            | uint64 |
| full\_offset    | Lowest block index                        | uint64 |
| items           | List of blocks                            | array  |
