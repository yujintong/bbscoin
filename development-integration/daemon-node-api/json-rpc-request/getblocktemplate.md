# getblocktemplate



### Input

| Argument        | Mandatory | Description                                 | Format |
| --------------- | --------- | ------------------------------------------- | ------ |
| reserve\_size   | yes       | Maximum of 255 bytes reserved for user data | uint64 |
| wallet\_address | yes       | Wallet address for block reward             | string |

### Output

| Argument            | Description                                       | Format |
| ------------------- | ------------------------------------------------- | ------ |
| difficulty          | Target difficulty                                 | uint64 |
| height              | Current block height                              | uint32 |
| num\_transactions   | Number of transactions included in block template | uint32 |
| reserved\_offset    | Offset of reserved space for user data            | uint64 |
| blocktemplate\_blob | Binary large object containing block template     | string |
| status              | Status of the request, "OK" if successful         | string |

### Notes

* num\_transactions can be used to discard block template if minimum number of transactions is not satisfied
