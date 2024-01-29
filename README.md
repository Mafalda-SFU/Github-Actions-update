# Github Actions init

Initialize Github Actions workflows for Node.js projects

Code checkout, setup SSH, setup Node.js and npm cache, install npm dependencies,
and install test reporters.

## inputs

All inputs are optional, using their default values if not provided.

- `node_auth_token`: Github authentication token for installing npm dependencies
  from Github Packages Registry.
- `node-version`: Node.js version to use.
- `ref`: Git ref to checkout.
- `ssh-private-key`: SSH private key for installing private git dependencies.
- `test-reporters`: Test reporters to install.
