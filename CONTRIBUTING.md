# Contributing Guidelines

Contributions are welcome via GitHub pull requests.
This document outlines the process to help get your contribution accepted.

## How to Contribute

1. Fork this repository, develop, and test your changes.
2. Submit a pull request with a clear description of what changed and why.
3. Keep pull requests focused; if possible, submit changes to multiple charts in separate PRs.

## Technical Requirements

- Follow [Helm chart best practices](https://helm.sh/docs/topics/chart_best_practices/).
- Ensure CI passes for linting and chart validation (including [chart-testing](https://github.com/helm/chart-testing) checks).
- Any change to a chart requires a version bump following [semver](https://semver.org/) principles.
- Update packaged chart artifacts and `index.yaml` when publishing a new chart version.

Once changes are merged, release/publishing automation (if configured) can package and publish updated charts.

## Immutability

Chart releases must be immutable.
Any change to a chart warrants a chart version bump, even when the change is documentation-only.

## Versioning

Chart `version` values should follow [semver](https://semver.org/).

For breaking (backward-incompatible) changes:

1. Bump the MAJOR version.
2. Document upgrade steps in the chart README under an `Upgrading` section.

## Updating Repository Index

When updating this chart repository manually:

1. Add the new packaged chart (`.tgz`) under the appropriate chart directory.
2. Re-generate the repository index with the repository URL set to `https://devolutions.github.io/helm-charts`.
3. Commit the updated package(s) and `index.yaml` in the same pull request.

## Community Expectations

Please be respectful and constructive in issues and pull requests.
By participating in this project, you agree to collaborate in good faith and follow GitHub community standards.
