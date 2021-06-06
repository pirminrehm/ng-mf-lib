# Angular Multi-Repo Webpack Module Federation Example (Micro Frontends)

## The Shared Lib

This repository is part of an Angular mlti-repo Webpack Module Federation example, explained [here](https://github.com/pirminrehm/ng-mf-shell#readme).

### Provide the Shared Lib

To provide the lib, run:

- `npm i`
- `npm run build`
- provide a local registray at port 4837, e.g. verdaccio via docker
  - `docker run --name verdaccio -p 4873:4873 -d verdaccio/verdaccio`
  - `npm login --registry http://localhost:4873`
- `npm run publish`

Now the lib should be published and you can proceed with thie installation of the other repos.
