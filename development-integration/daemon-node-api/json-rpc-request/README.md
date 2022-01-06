# JSON RPC request



### Usage

#### Using cURL

* curl -X POST http://127.0.0.1:21204/json\_rpc -H 'Content-Type: application/json-rpc' -d '{"jsonrpc": "2.0", "method": "getcurrencyid", "params": {}, "id": "1"}'
* curl -X POST http://127.0.0.1:21204/json\_rpc -H 'Content-Type: application/json-rpc' -d '{"jsonrpc": "2.0", "method": "getblockheaderbyheight", "params": {"height" : 0}, "id": "1"}'
