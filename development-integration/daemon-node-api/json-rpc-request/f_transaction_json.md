# f\_transaction\_json

### Input

| Argument | Mandatory | Description      | Format |
| -------- | --------- | ---------------- | ------ |
| hash     | yes       | Transaction hash | string |

### Output

| Argument  | Description                               | Format |
| --------- | ----------------------------------------- | ------ |
| tx        | Transaction                               | struct |
| txDetails | Transaction details                       | struct |
| block     | Block                                     | struct |
| status    | Status of the request, "OK" if successful | string |
