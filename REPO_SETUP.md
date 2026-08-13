# Repository setup — when ready to test on GitHub

You do **not** need to create repositories before reviewing the local V1.

When V1 is accepted, create:

1. `jlblancoupm/jlblancoupm.github.io` — public website repository.
2. `jlblancoupm/profile-data` — private canonical-data repository.

For the website repository:

- default branch: `main`
- Settings → Pages → Source: **GitHub Actions**
- protect `main` so normal updates arrive through pull requests
- do not store private canonical YAML, CV generators, secrets or Telegram credentials in this repository

The private `profile-data` repository will later contain the sync jobs, review candidates, overrides, sanitization/export logic and Telegram notification secret.
