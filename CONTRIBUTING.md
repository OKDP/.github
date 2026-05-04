# Contributing to OKDP

Thank you for your interest in contributing to OKDP!

## How to Contribute

### Reporting Issues

- Use GitHub Issues on the relevant repository
- Use the provided issue templates (bug report, feature request)
- For security vulnerabilities, see [SECURITY.md](SECURITY.md)

### Contributing Documentation

- Follow the existing repository structure and naming conventions
- Use the provided templates when available
- Keep guides focused on one component

### Contributing Code

The workflow depends on the visibility of the target repository.

#### Public repositories (open-source contribution)

The default workflow for everyone is **fork-based**:

1. **Fork** the repository on GitHub
2. Clone your fork and create a feature branch from `main`
3. Make your changes
4. Ensure CI passes, if configured (lint, tests, build...)
5. Submit a Pull Request from your fork to the upstream `main`
6. The Pull Request must be related to an issue

> **Maintainers only (urgent/quick fixes):** maintainers may create a branch directly in the upstream repository instead of forking, but only for time-sensitive changes. The fork-based workflow remains the default for all other contributions.

#### Private repositories (internal team contribution)

1. Create a branch **directly from `main`** in the repository (no fork needed)
2. Make your changes
3. Ensure CI passes, if configured (lint, tests, build)
4. Submit a Pull Request to `main`
5. The Pull Request must be related to an issue

### Commit Messages

Follow [Conventional Commits](https://www.conventionalcommits.org/):

```
feat: add OIDC support for Trino
fix: correct S3 endpoint in hive-metastore values
docs: update airflow INSTALL.md with gitSync config
chore: bump cert-manager to v1.17.1
```

### Pull Request Process

- Bug fixes and minor changes require at least 1 maintainer approval (lazy consensus)
- Feature PRs and documentation PRs are reviewed and approved at the **TOSIT Contributors Meeting**. Please, plan your submissions accordingly
- All CI checks must pass if configured
- Keep PRs focused, one change per PR
- Before merge, **squash your commits** into meaningful units and **rebase your branch** on top of the latest `main`. Use `git push --force-with-lease` to update the PR.

## Getting Help

For questions, ideas, or technical discussions, use [OKDP GitHub Discussions](https://github.com/orgs/OKDP/discussions).

## Repository Map

| Repository                                                  | What to Contribute                             |
| ----------------------------------------------------------- | ---------------------------------------------- |
| [OKDP/OKDP](https://github.com/OKDP/OKDP)                   | Project-level docs, governance, roadmap        |
| [OKDP/helm-handbook](https://github.com/OKDP/helm-handbook) | Helm chart install guides and values           |
| [OKDP/okdp-sandbox](https://github.com/OKDP/okdp-sandbox)   | Sandbox environment                            |
| OKDP/hive-metastore, spark-history-server, etc.             | Module source code, Helm charts, Docker images |

## Contributor License Agreement (CLA)

Before your first contribution can be merged, you must sign the OKDP CLA (one-time requirement).

<!-- TODO: add link to CLA signing process once finalized -->

## Code of Conduct

This project follows the [Contributor Covenant Code of Conduct](CODE_OF_CONDUCT.md).