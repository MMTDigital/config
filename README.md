## Cutting a Release

1. Tag all merged pull requests that go into the release with the relevant milestone. Each merged PR should also be labeled with one of the [labels](https://github.com/MMTDigital/config/labels) named `tag: ...` to indicate what kind of change it is.

2. Create a change log entry for the release:

- You'll need an [access token for the GitHub API](https://help.github.com/articles/creating-an-access-token-for-command-line-use/). Save it to this environment variable: `export GITHUB_AUTH="..."`
- Run `yarn changelog`. The command will find all the labeled pull requests merged since the last release and group them by the label and affected packages, and create a change log entry with all the changes and links to PRs and their authors. Copy and paste it to `CHANGELOG.md`.
