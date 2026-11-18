<p align="center"><img src="https://raw.githubusercontent.com/Iridium-Group/.github/main/assets/iridium-mark.svg" width="96" alt="Iridium Group"></p>

# Iridium Group

> Technology for a more open web.

Iridium Group is an independent open-source technology collective focused on building fast, reliable, and accessible web infrastructure. We build open web infrastructure for browser-based networking and proxy applications, together with the small libraries, tools, and documentation that support it.

## Projects

All projects are at version 0.1.0. None of them is stable yet, and their APIs may change between releases.

| Repository                                                              | Description                                                                            | Status       |
| ----------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | ------------ |
| [iridium](https://github.com/Iridium-Group/iridium)                     | The Iridium Group website and the shared UI styles and components in its `ui/` folder. | Development  |
| [iridium-docs](https://github.com/Iridium-Group/iridium-docs)           | Documentation for Iridium Group projects.                                              | Development  |
| [iridium-proxy](https://github.com/Iridium-Group/iridium-proxy)         | A self-hostable proxy server for browser-based networking, with Wisp support.          | Experimental |
| [iridium-transport](https://github.com/Iridium-Group/iridium-transport) | A transport abstraction with direct, Wisp client, and in-memory implementations.       | Experimental |
| [iridium-utils](https://github.com/Iridium-Group/iridium-utils)         | Zero-dependency helpers for URLs, encoding, JSON, headers, timing, and address checks. | Experimental |
| [iridium-config](https://github.com/Iridium-Group/iridium-config)       | Schema, validation, and loading for Iridium configuration files.                       | Experimental |
| [iridium-inspector](https://github.com/Iridium-Group/iridium-inspector) | A browser-based diagnostics tool for URLs, headers, and encoded data.                  | Experimental |
| [iridium-examples](https://github.com/Iridium-Group/iridium-examples)   | Small, runnable examples that use the Iridium libraries.                               | Development  |
| [iridium-status](https://github.com/Iridium-Group/iridium-status)       | A status page for Iridium Group services.                                              | Development  |

## Infrastructure

Our technical work centers on a few connected areas:

- **Transport abstraction.** A single `Transport` interface lets the same code open connections directly from Node.js, over a Wisp connection from the browser, or in memory for tests.
- **Wisp-based browser networking.** Browsers cannot open raw TCP sockets, so we multiplex streams over a WebSocket using the Wisp protocol, which was created by Mercury Workshop.
- **Proxy infrastructure.** Self-hostable servers with safe defaults: private and internal addresses are blocked, outbound mail ports are refused by default, and connection limits and idle timeouts are enforced.
- **Diagnostics.** Health and readiness endpoints, structured logging that leaves out destinations by default, and tools for inspecting what a request actually sends.

## Open source

Everything we build is developed in public and released under an open-source license. We keep runtime dependencies to a minimum, document the licenses of the dependencies we do use, and credit the upstream projects we build on.

- Iridium Group projects are licensed under the MIT License.
- The exception is iridium-proxy, which is licensed under AGPL-3.0-only because it bundles AGPL-3.0-licensed components.

Each repository's README lists its dependencies and their licenses.

## Community

We use GitHub for all project communication. There is no Discord server, mailing list, or other chat channel.

- **Issues:** report bugs and request features in the issue tracker of the relevant repository.
- **Discussions:** GitHub Discussions will be enabled on the `.github` repository for questions and general conversation.
- **Security:** report vulnerabilities privately, as described in our [security policy](https://github.com/Iridium-Group/.github/blob/main/SECURITY.md). Please do not open public issues for security problems.

Everyone taking part is expected to follow our [Code of Conduct](https://github.com/Iridium-Group/.github/blob/main/CODE_OF_CONDUCT.md).

## Contributing

Contributions are welcome, from typo fixes to new features. Start with the [contributing guide](https://github.com/Iridium-Group/.github/blob/main/CONTRIBUTING.md), which covers local setup, tests, formatting, commit messages, and how pull requests are reviewed. For larger changes, please open an issue first so we can agree on the approach.
