---
description: >-
  Either spendSecretKey or spendPublicKey, or neither, should be specified. New
  keys will be generated if neither parameter is specified.
---

# createAddress

### Input

| Argument       | Mandatory | Description             | Format |
| -------------- | --------- | ----------------------- | ------ |
| spendSecretKey | no        | Secret spend key to use | string |
| spendPublicKey | no        | Public spend key to use | string |

### Output

| Argument | Description                | Format |
| -------- | -------------------------- | ------ |
| address  | Address for created wallet | string |
