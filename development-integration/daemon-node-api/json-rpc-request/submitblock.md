# submitblock



### Input

| Argument | Mandatory | Description                     | Format                      |
| -------- | --------- | ------------------------------- | --------------------------- |
|          | yes       | Binary array of block to submit | array of hexadecimal string |

### Output

| Argument | Description                           | Format |
| -------- | ------------------------------------- | ------ |
| status   | Status of request, "OK" if successful | string |

### Notes

* This method expects an array containing single element of hexadecimal string converted from block data.
