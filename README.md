# Reproduction case for an `@effect/docgen` issue

This repository contains a simple reproduction case for an `@effect/docgen` [bug](https://github.com/Effect-TS/docgen/issues/93) where JSDoc examples of namespaced `type` objects are not being typechecked.

## Reproduction steps

1. Clone this repo
2. `pnpm install`
3. `pnpm docgen`

Step 3 should fail but instead it succeeds and produces a [document](./docs/modules/index.ts.md) containing a code example that does not typecheck.
