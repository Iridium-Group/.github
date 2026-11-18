# Contributing to Iridium Group

Thank you for your interest in contributing. This guide applies to every repository in the Iridium Group organization. Some repositories add their own `CONTRIBUTING.md` with project-specific commands; when they do, follow both.

By taking part, you agree to follow our [Code of Conduct](./CODE_OF_CONDUCT.md).

## Before you start

- For bugs, search the repository's existing issues first, then open a bug report if none matches.
- For new features or larger changes, open an issue describing the problem before writing code, so we can agree on the approach.
- For security problems, do not open an issue. Follow the [security policy](./SECURITY.md) instead.

## Requirements

- Node.js 22.18 or later
- npm (the version that ships with Node.js). Iridium Group projects use npm; please do not commit lockfiles from other package managers.
- Git

## Set up

Fork the repository on GitHub, then clone your fork. Replace `<you>` with your GitHub username and `<repo>` with the repository name:

```sh
git clone https://github.com/<you>/<repo>.git
cd <repo>
npm ci
```

`npm ci` installs the exact versions recorded in `package-lock.json`. Use `npm install` only when you intend to change dependencies.

## Run locally

Most repositories provide these scripts:

| Command                | What it does                                      |
| ---------------------- | ------------------------------------------------- |
| `npm run build`        | Compiles TypeScript into `dist/`.                 |
| `npm test`             | Runs the test suite with the Node.js test runner. |
| `npm run typecheck`    | Type-checks the code without emitting output.     |
| `npm run format`       | Formats the code with Prettier.                   |
| `npm run format:check` | Checks formatting without changing files.         |

Applications and sites may add a `dev` script or other commands. Check the repository's README for those.

## Test

Run the full check before opening a pull request. These are the same steps CI runs:

```sh
npm run format:check
npm run typecheck
npm test
npm run build
```

Add or update tests for any change in behavior. Tests live in `test/` and use `node:test` and `node:assert`.

## Format

Code is formatted with [Prettier](https://prettier.io), using the `.prettierrc` in each repository. Run `npm run format` before committing. Pull requests that fail `npm run format:check` will not pass CI.

## Code style

- TypeScript in strict mode, ESM only.
- Library repositories have no runtime dependencies. Discuss any new dependency in an issue first.
- US English in code and identifiers; plain, clear English in documentation.
- Never commit secrets, tokens, `.env` files, `node_modules`, or build output.

## Issues

Use the issue forms provided in each repository. A good bug report includes the version, your environment, exact steps to reproduce, what you expected, and what happened instead. Keep each issue to one problem.

## Pull requests

1. Create a branch from `main` in your fork.
2. Make focused changes. Separate unrelated changes into separate pull requests.
3. Run the checks above and make sure they pass.
4. Update documentation and `CHANGELOG.md` when your change affects users.
5. Open a pull request against `main` and fill in the template.

Small fixes such as typos can go straight to a pull request without an issue.

## Commit messages

We use [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/). Each commit message starts with a type and a short summary in the imperative mood:

```text
feat: add base64url helpers
fix: reject IPv4-mapped private addresses
docs: explain transport configuration
```

Common types are `feat`, `fix`, `docs`, `chore`, `ci`, `test`, and `refactor`. Mark breaking changes with `!` after the type (for example `feat!:`) and explain them in the commit body.

## Review

- A maintainer reviews every pull request before it is merged. Iridium Group is run by volunteers, so reviews can take some time; a polite reminder after a week is welcome.
- CI must pass before merging.
- Reviewers may ask for changes. Push follow-up commits to the same branch rather than opening a new pull request.
- Maintainers may squash commits when merging, so the pull request title should also follow Conventional Commits.

## Developer Certificate of Origin

A Developer Certificate of Origin (DCO) sign-off is not required. By submitting a pull request, you agree that your contribution is licensed under the license of the repository you are contributing to.

## Licensing

Iridium Group projects are licensed under the MIT License, except iridium-proxy, which is licensed under AGPL-3.0-only. Check the `LICENSE` file in the repository you are contributing to.
