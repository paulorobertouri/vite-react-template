# vite-react-template

Modern React + TypeScript template focused on clean domain logic, fast feedback, and maintainability.

## Stack

- Vite + React + TypeScript
- Vitest + Testing Library
- ESLint + Prettier
- VS Code debug profiles

## Commands

- `pnpm install`
- `pnpm dev`
- `pnpm test`
- `pnpm test:coverage`
- `pnpm lint`
- `pnpm format`

## Architecture

- `src/domain`: pure business rules (easy to test)
- `src`: UI composition and styling
- `tests`: component and domain tests

This template follows Fowler-style separation of domain logic from presentation concerns.

## Shared Template Contract

All frontend templates in this repository follow the same functional contract and quality gates.

### Functional Contract

- Deliver the same Task Board behavior:
	- Add a task from input
	- Toggle completion state
	- Remove a task
- Keep business rules in a pure domain module.
- Keep UI concerns in framework-specific components.

### Quality Gates

- Lint must pass.
- Typecheck must pass.
- Unit tests must pass.
- Component behavior tests must pass.

### Architecture Contract

- Domain logic: pure functions, no framework dependencies.
- Presentation layer: state wiring, rendering, and event orchestration.
- Tests: domain tests + UI behavior tests.

This is the common baseline across React, Preact, WXT React, and Angular templates.
