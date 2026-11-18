# Security policy

This policy applies to every repository in the Iridium Group organization unless a repository provides its own `SECURITY.md`.

## Supported versions

All Iridium Group projects are in early development (0.x). Only the latest released 0.x version of each project receives security fixes. Fixes are not backported to earlier versions.

| Version              | Supported |
| -------------------- | --------- |
| Latest 0.x release   | Yes       |
| Earlier 0.x releases | No        |

## Reporting a vulnerability

Please do not report security vulnerabilities through public issues, discussions, or pull requests.

Iridium Group does not have a security email address. Report vulnerabilities through GitHub private vulnerability reporting on the affected repository:

1. Open the affected repository on GitHub.
2. Go to the **Security** tab.
3. Select **Report a vulnerability**.
4. Fill in the form and submit it.

The report is visible only to you and the repository's maintainers. GitHub describes the process in [Privately reporting a security vulnerability](https://docs.github.com/en/code-security/security-advisories/guidance-on-reporting-and-writing-information-about-vulnerabilities/privately-reporting-a-security-vulnerability).

If you are not sure which repository is affected, report it on the repository you think is most likely and say so in the report.

## What to include

- The affected repository and version, or the commit you tested.
- A description of the vulnerability and its impact.
- Step-by-step instructions to reproduce it, including any configuration needed.
- A proof of concept, if you have one.
- Any suggested fix or mitigation.

Please test only against your own deployments. Do not access, change, or delete data that is not yours, and do not degrade services run by others.

## What to expect

Iridium Group is maintained by volunteers. These are goals, not guarantees:

- We aim to acknowledge a report within 7 days.
- We aim to share an initial assessment within 14 days.
- We will keep you informed as we work on a fix, and we will tell you if we decide the report is not a vulnerability.
- Once a fix is released, we will publish a security advisory on the affected repository. We will credit you in the advisory if you would like to be credited.

Please keep the details private until a fix is released or we have agreed on a disclosure date with you.
