# Security policy

This policy covers each repository of the lmodel organisation that has no `SECURITY.md` of its own. A repository's own `SECURITY.md` takes precedence over it.

## Reporting a vulnerability

Use GitHub's private vulnerability reporting on the affected repository, under its Security tab, not a public issue or a pull request. State the repository and the file, how the flaw is exploitable, and whether it reaches a release or only the repository's automation. One person maintains these repositories. Expect a first reply in days, not hours. There is no bounty.

## Supported versions

Only the latest release of a repository receives fixes. A fix is released as a patch and noted in that repository's changelog.

## What this policy covers

- The code, workflows and releases each repository holds.
- The measures the repositories share, which the [threat model](https://github.com/noelmcloughlin/knowledge-trust-ladder/blob/main/docs/threat-model.md) sets out with its reasoning.

## Not covered

- The code a fork carries from its upstream project. Report a flaw in it to that project.
- A standard, vocabulary or dataset that a schema models. Report a problem in it to its publisher.
- LinkML, its generators and its runtime. Report a flaw in them to [LinkML](https://github.com/linkml/linkml/security).
