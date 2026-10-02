# AI Elements

A pnpm monorepo for React components and examples used to build AI interfaces, plus a documentation/demo app. The workspace contains `@repo/elements`, `@repo/examples`, `@repo/shadcn-ui`, a CLI, scripts, and shared TypeScript configuration.

## Requirements

- Node.js `>=20.12`
- pnpm `10.28.0`, declared in the root package manifest

## Develop

```bash
corepack enable
pnpm install
pnpm --filter docs dev
```

The docs app runs through its own Next.js scripts. Root scripts also expose workspace build, development, tests, coverage, lint/check, and formatting tasks.

## Verify

```bash
pnpm build --filter ai-elements --filter docs
pnpm test
```

These commands mirror the checked-in CI workflow. They were not run as part of this documentation change. Browser-based component tests may require Playwright browsers; see the CI workflow.

## Repository map

- `apps/docs/`: Next.js documentation and demo app
- `packages/elements/`: React AI interface components
- `packages/examples/`: example implementations
- `packages/cli/`: component-related CLI package
- `packages/shadcn-ui/`: shared UI components
- `packages/scripts/`: repository scripts, including skill generation
- `.changeset/`: package versioning and release metadata
- `.github/workflows/`: build/test, release, and skill-generation workflows

See the [documentation index](docs/README.md), [contribution guide](.github/CONTRIBUTING.md), and [security policy](.github/SECURITY.md).

## Releases and status

The root workspace is private. Individual packages have their own publish configuration and version metadata. The Changesets release workflow describes the publishing process; a workflow file alone does not prove a release or deployment succeeded.

## Scope

This repository provides UI components and example/docs applications. It does not provide a hosted model backend, a general-purpose agent orchestrator, or automatic model routing. Integrating applications choose their own AI SDK/provider and data handling.
