<p align="center"><img src="./assets/iridium-mark.svg" width="96" alt="Iridium Group"></p>

# .github

Shared configuration and community standards for Iridium Group projects.

This repository is the organization-wide `.github` repository for [Iridium Group](https://github.com/Iridium-Group). GitHub reads it in two ways: the `profile/` folder becomes the organization's public profile page, and the community health files below act as defaults for every public repository in the organization that does not provide its own copy.

## How GitHub inherits these files

- A repository in the organization that has no file of its own (in its root, `docs/`, or `.github/` folder) shows the version from this repository instead. For example, every Iridium Group repository links to [SECURITY.md](./SECURITY.md) here unless it adds a repository-specific policy.
- A repository's own file always takes precedence over the organization default. Defaults are not copied into repositories; they are read from here when needed.
- Issue templates and `config.yml` in `.github/ISSUE_TEMPLATE/` are inherited only by repositories that have no `.github/ISSUE_TEMPLATE/` folder of their own.
- `LICENSE` files are not inherited. Each repository carries its own license.
- Workflow templates in `workflow-templates/` are not applied automatically. They appear in each repository's Actions tab under "New workflow", where a maintainer can choose to add them.
- Files only apply to public repositories, because this repository is public.

GitHub documents this behavior in [Creating a default community health file](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/creating-a-default-community-health-file).

## Contents

| Path                                                                           | Purpose                                                                                                                               |
| ------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------- |
| [`profile/README.md`](./profile/README.md)                                     | The organization profile shown at <https://github.com/Iridium-Group>.                                                                 |
| [`CONTRIBUTING.md`](./CONTRIBUTING.md)                                         | How to set up, test, format, and submit changes to any Iridium Group repository.                                                      |
| [`CODE_OF_CONDUCT.md`](./CODE_OF_CONDUCT.md)                                   | Contributor Covenant 2.1, with how to report conduct issues.                                                                          |
| [`SECURITY.md`](./SECURITY.md)                                                 | Supported versions and how to report a vulnerability privately.                                                                       |
| [`SUPPORT.md`](./SUPPORT.md)                                                   | Where to ask questions and report problems.                                                                                           |
| [`.github/ISSUE_TEMPLATE/`](./.github/ISSUE_TEMPLATE)                          | Default issue forms (bug report, feature request), a security notice that points to private reporting, and the chooser configuration. |
| [`.github/pull_request_template.md`](./.github/pull_request_template.md)       | Default pull request description.                                                                                                     |
| [`.github/workflows/lint-markdown.yml`](./.github/workflows/lint-markdown.yml) | Lints the Markdown in this repository and checks its external links.                                                                  |
| [`workflow-templates/`](./workflow-templates)                                  | The standard Iridium Node.js CI workflow, offered in each repository's Actions tab.                                                   |
| [`assets/`](./assets)                                                          | The Iridium mark and avatar, with usage notes in [`BRAND.md`](./assets/BRAND.md).                                                     |
| [`LICENSE`](./LICENSE)                                                         | MIT license for the contents of this repository.                                                                                      |

There is no `FUNDING.yml`, because Iridium Group does not accept funding at this time.

## Checking changes locally

The workflow in `.github/workflows/lint-markdown.yml` runs [markdownlint-cli2](https://github.com/DavidAnson/markdownlint-cli2) with the rules in `.markdownlint-cli2.jsonc`. To run the same lint before pushing:

```sh
npx markdownlint-cli2
```

## License

The contents of this repository are available under the [MIT License](./LICENSE).
