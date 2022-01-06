# getinfo

### Input

| Argument | Mandatory | Description | Format |
| -------- | --------- | ----------- | ------ |
| none     |           |             |        |

### Output

| Argument                     | Description                                           | Format |
| ---------------------------- | ----------------------------------------------------- | ------ |
| status                       | Status of the request, "OK" if successful             | string |
| height                       | Blockchain height                                     | uint64 |
| difficulty                   | Difficulty of latest block                            | uint64 |
| tx\_count                    | Cumulative number of transactions since genesis block | uint64 |
| tx\_pool\_size               | Number of unconfirmed transactions in pool            | uint64 |
| alt\_blocks\_count           | Number of blocks in alternate chains                  | uint64 |
| outgoing\_connections\_count | Number of outgoing connections                        | uint64 |
| incoming\_connections\_count | Number of incoming connections                        | uint64 |
| white\_peerlist\_size        | Number of peers in white list                         | uint64 |
| grey\_peerlist\_size         | Number of peers in grey list                          | uint64 |
| last\_known\_block\_index    | Last known block index                                | uint32 |
| network\_height              | Remote network blockchain height                      | uint32 |
| hashrate                     | Estimated hash rate of latest block                   | uint32 |
| version                      | Daemon version                                        | string |
| synced                       | Is the local daemon synced with network               | bool   |
| fee\_address                 | Fee address of local daemon                           | string |
| max\_block\_size             | Maximum size for new block                            | uint64 |
| max\_tx\_size                | Maximum size for new transaction                      | uint64 |
| genesis\_time                | Time stamp of genesis block                           | uint64 |

### Usage

#### cURL

* curl http://127.0.0.1:21204/getinfo
