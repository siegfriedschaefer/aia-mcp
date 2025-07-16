# aia-mcp
AIA's mcp server

## how to test with echo command
```bash
echo '{"jsonrpc":"2.0","method":"foo","id":1}' | node build/index.js | jq .

