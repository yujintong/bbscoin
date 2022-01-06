# get\_blocks\_hashes\_by\_timestamps.bin

### Input

| Argument       | Mandatory | Description                                   | Format |
| -------------- | --------- | --------------------------------------------- | ------ |
| timestampBegin | yes       | Time stamp to start                           | uint64 |
| secondsCount   | yes       | Number of seconds after timestampBegin to end | uint64 |

### Output

| Argument    | Description                               | Format |
| ----------- | ----------------------------------------- | ------ |
| blockHashes | List of block hashes                      | array  |
| status      | Status of the request, "OK" if successful | string |
