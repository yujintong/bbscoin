# getheight

### Input

| Argument | Mandatory | Description | Format |
| -------- | --------- | ----------- | ------ |
| none     |           |             |        |

### Output

| Argument        | Description                           | Format |
| --------------- | ------------------------------------- | ------ |
| height          | Local blockchain height               | uint64 |
| network\_height | Network blockchain height             | uint32 |
| status          | Status of request, "OK" if successful | string |

### Usage

#### cURL

* curl http://127.0.0.1:21204/getheight
