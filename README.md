# `bun-8761-repro-snapshot`

Repro for: <https://github.com/oven-sh/bun/issues/8761>

## Repro steps

```shell
git clone https://github.com/lgarron/bun-8761-repro-snapshot && cd bun-8761-repro-snapshot
bun install
bun x tsc
```

## Creation

This repo was created by running:

```
mkdir /tmp/bun-node-types && cd /tmp/bun-node-types
bun init --yes
bun add @types/node @types/bun typescript
echo "{}" > tsconfig.json # Remove `skipLibCheck`
```
