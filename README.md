# Composer Registry

## Add Package

- Update `repositories` in `satis.json` with the GitHub repository URL of the new package.

## Automation

- The following GitHub secrets must be defined:

  - `PACKAGE_READ_TOKEN` with a GitHub token that has read access to all included repositories.

  - `DEPLOY_PRIVATE_KEY` with an SSH private key that has write access to the deployment server.

- The [`build.yml` workflow](.github/workflows/build.yml) is triggered on push to the `main` branch.