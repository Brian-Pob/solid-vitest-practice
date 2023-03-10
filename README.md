# Solid Vitest Practice

Practice project for vitest and solidjs.

## Issues

Vitest on watch mode shows all tests as failing after any change in the code.

[Demo video](https://share.cleanshot.com/fZD758Yy)

- Environment:
  - Mac OS 13.2.1
  - Node 19.6.0
  - pnpm 7.27.0
- Additional environents:
  - GitPod
    - Node 16.19.0
    - pnpm 7.22.0
  - CodeSandbox Cloud Sandbox
    - Node 16.17.0
    - pnpm 7.1.0
- Steps to reproduce:
  1. `pnpm i`
  2. `pnpm test`
      - All tests should pass

  3. Make a valid change in `todo-list.tsx` and save.
     - Expected: All tests should pass
     - Observed: All tests fail

  4. Undo change. Resetting the file to the original state.
     - Expected: All tests should pass
     - Observed: All tests fail

  5. Stop the test runner and start it again.
     - All tests pass
