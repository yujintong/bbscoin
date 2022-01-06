# getblockheaderbyheight

### Input

| Argument | Mandatory | Description                          | Format |
| -------- | --------- | ------------------------------------ | ------ |
| height   | yes       | Block height of the block to request | uint64 |

### Output

| Argument      | Description                               | Format |
| ------------- | ----------------------------------------- | ------ |
| block\_header | Block header                              | struct |
| status        | Status of the request, "OK" if successful | string |
