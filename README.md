# aia-mcp
AIA's mcp server

## how to test with echo command
```bash
cd server
echo '{"jsonrpc":"2.0","method":"foo","id":1}' | node build/index.js | jq .
```

## how to build monorepo

* build mcp server
```bash
npm run build -w server
```

* build mcp client
```bash
npm run build -w client
```

## how to start a minimalistic 'stdio' mcp client
Since we are building a local 'stdio' client, the client has to fork the mcp server
```bash
node client/build/index.js
```
