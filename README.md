# `valentjn/renovate`

This repository contains a GitHub Actions workflow that runs Renovate on select `valentjn` repositories. The workflow is run weekly and can be triggered manually.

## Adding a Repository

1. Make sure that pull requests are enabled in the settings of the repository to be added (can be set to collaborator only). Otherwise, Renovate will error.
2. Add the repository to the PAT [`VALENTJN_RENOVATE_PAT`](https://github.com/settings/personal-access-tokens/13129399).
3. Add the repository to [`renovate-self-hosted.json`](renovate-self-hosted.json) in this repository.
