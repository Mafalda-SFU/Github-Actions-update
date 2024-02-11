# Github Actions update

Update version and dependencies Node.js projects

1. Update source code with provided script
2. Update package version
3. Update specified dependencies to their latest version
4. Update other dependencies to the latest semver compatible version
5. Install updated dependencies and update lockfile
6. Run tests with updated dependencies to detect regressions
7. Commit changes and push to the repository

## inputs

All inputs are optional, using their default values if not provided.

- `dependencies-update-latest`: List of dependencies to update to their latest
  version. Default: `[]`
- `new_version`: New version to set in `package.json`.
- `node_auth_token`: Github authentication token for installing npm dependencies
  from Github Packages Registry.
- `reference-package-name`: Name of the package to use as reference for updating
  other dependencies.
- `update-script`: Script to update source code.
- `user-email`: Email to use for the commit. Default: Github Actions bot email
- `user-name`: Name to use for the commit. Default: Github Actions bot name
