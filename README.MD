# vite-react-template

Modern React + TypeScript template with a clear separation between domain and UI logic.

## Stack

- Vite + React + TypeScript
- Vitest + Testing Library
- ESLint + Prettier
- VS Code debug profiles

## Commands

- `make install` — install dependencies
- `make install-dev` — install dev dependencies
- `make dev` — start dev server
- `make build` — build for production
- `make test` — run tests
- `make format` — format code
- `make preview` — preview production build

## Project Structure

```text
.
├── src/
│   ├── domain/          # pure business rules
│   ├── App.tsx          # root component
│   ├── App.css
│   └── index.css
├── tests/
├── scripts/
│   ├── ubuntu/
│   └── windows/
└── Makefile
```

## Architecture

- `src/domain`: pure business rules, framework-agnostic
- `src`: rendering and interactions
- `tests`: domain tests and UI tests

Follows Fowler-style separation of concerns; side effects stay at the boundaries.

## Functional Contract

- Task Board: add, toggle, and remove tasks.
- Business rules live in the domain module.
- UI concerns stay in framework-specific components.

## Quality Gates

- Lint must pass.
- Typecheck must pass.
- Unit tests must pass.
- Component behavior tests must pass.
