# getblockheaderbyhash

### Input

| Argument | Mandatory | Description                        | Format |
| -------- | --------- | ---------------------------------- | ------ |
| hash     | yes       | Block hash of the block to request | string |

### Output

| Argument      | Description                               | Format |
| ------------- | ----------------------------------------- | ------ |
| block\_header | Block header                              | struct |
| status        | Status of the request, "OK" if successful | string |
