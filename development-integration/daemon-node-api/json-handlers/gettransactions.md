# gettransactions

### Input

| Argument    | Mandatory | Description                | Format |
| ----------- | --------- | -------------------------- | ------ |
| txs\_hashes | yes       | List of transaction hashes | array  |

### Output

| Argument     | Description                           | Format |
| ------------ | ------------------------------------- | ------ |
| txs\_as\_hex | List of transactions blobs as hex     | array  |
| missed\_tx   | List of transactions not found        | array  |
| status       | Status of request, "OK" if successful | string |

### Notes

* Transaction hashes are passed as strings
