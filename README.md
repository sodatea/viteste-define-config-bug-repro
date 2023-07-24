# viteste-define-config-bug-repro

First, install the dependencies:

```sh
pnpm i
```

To reproduce the bug, run the following commands:

```sh
pnpm patch-remove vitest@0.33.0
pnpm type-check
```

To restore the patch to see the fixed version:

```sh
git restore -- .
pnpm i
pnpm type-check
```
