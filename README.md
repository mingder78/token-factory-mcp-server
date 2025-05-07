# token-factory-mcp-server

## build

To install dependencies:

```bash
bun i
```

To run:

```bash
bun dev
```

## inspector (test)

```bash
bun inspector
```

This project was created using `bun init` in bun v1.2.9. [Bun](https://bun.sh) is a fast all-in-one JavaScript runtime.

# mcp client config

```json
{
  "mcpServers": {
    "token-factory-mcp-server": {
      "command": "npx",
      "args": ["token-factory-mcp-server@latest"]
    }
  }
}
```

* for developers

```sh
bun run build
```

```json
 "token-factory-mcp-server": {
      "command": "node",
      "args": ["/tmp/token-factory-mcp-server/build/index.js"]
    }
```

## deployment

```sh
npm publish --public

> token-factory-mcp-server@0.0.2 prepare
> npm run build


> token-factory-mcp-server@0.0.2 build
> tsc && node -e "require('fs').chmodSync('build/index.js', '755')"

npm notice
npm notice 📦  token-factory-mcp-server@0.0.2
npm notice Tarball Contents
npm notice 391B README.md
npm notice 29B agents/evaluator.ts
npm notice 969B build/index.js
npm notice 588B package.json
npm notice 0B routes/ask-agent.ts
npm notice 844B src/index.ts
npm notice 765B tsconfig.json
npm notice 26B utils/github.ts
npm notice Tarball Details
npm notice name: token-factory-mcp-server
npm notice version: 0.0.2
npm notice filename: token-factory-mcp-server-0.0.2.tgz
npm notice package size: 1.7 kB
npm notice unpacked size: 3.6 kB
npm notice shasum: c422ba922c58752985dff94762b95596ac4bebcf
npm notice integrity: sha512-vd7v9k0NJo1Vz[...]g9V/YKZE+jrYQ==
npm notice total files: 8
npm notice
npm notice Publishing to https://registry.npmjs.org/ with tag latest and default access
+ token-factory-mcp-server@0.0.2
```
