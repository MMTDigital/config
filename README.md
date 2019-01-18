
# MMTDigital Config

## Quick Overview

## Contributing

```bash
  npm install -g lerna
  
```

Clone the repo with git clone https://github.com/MMTDigital/config

```bash
  lerna bootstrap
```

## Submitting a Pull Request

Good pull requests, such as patches, improvements, and new features, are a fantastic help. They should remain focused in scope and avoid containing unrelated commits.

In order to help generate useful documentation we're adhereing to https://www.conventionalcommits.org/en/v1.0.0-beta.2/

## Cutting a Release

1. Each PR should also be labeled with one of the [labels](https://github.com/MMTDigital/config/labels) named `tag: ...` to indicate what kind of change it is.

2. Create a change log entry for the release:

- You'll need an [access token for the GitHub API](https://github.com/settings/tokens/new?description=GitHub%20Changelog%20Generator%20token). Since this is a public repository, you only need `public_repo` access for the token. Save it to this environment variable: `export GITHUB_AUTH="..."`
- Run `yarn changelog`. The command will find all the labeled pull requests merged since the last release and group them by the label and affected packages, and create a change log entry with all the changes and links to PRs and their authors. Copy and paste it to `CHANGELOG.md`.
