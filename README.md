# Composer Registry

## Add Package

- Update `repositories` in `satis.json` with the GitHub repository URL of the new package.

## Automation

- GitHub Secret `PACKAGE_READ_TOKEN` must contain a token that has read access to all included repositories.

- The [`build.yml` workflow](.github/workflows/build.yml) is triggered on push to the `main` branch.