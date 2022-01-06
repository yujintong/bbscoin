---
description: >-
  This method stops the daemon. Stopping the daemon is only allowed if the
  daemon is running on testnet.
---

# stop\_daemon

### Input

| Argument | Mandatory | Description | Format |
| -------- | --------- | ----------- | ------ |
| none     |           |             |        |

### Output

| Argument | Description                               | Format |
| -------- | ----------------------------------------- | ------ |
| status   | Status of the request, "OK" if successful | string |

### Usage

#### cURL

* curl http://127.0.0.1:21204/stop\_daemon
