# Project conventions

## Runtime
- Scripts are executed with `tsx` (not compiled to JS)
- `noEmit: true` in tsconfig is intentional — no build step

## Scripts
- `pnpm dev` — run `src/index.ts` in watch mode
- `pnpm test` — run tests once with vitest
- `pnpm lint` — eslint
- `pnpm format` — prettier
- `pnpm typecheck` — tsc type check only

## Tests
- Test files live alongside source files (`foo.ts` / `foo.spec.ts`)
- Import from vitest explicitly: `import { describe, expect, it } from "vitest"`

## Package manager
- Use `pnpm` exclusively
