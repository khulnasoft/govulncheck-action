# Easily using govulncheck in GitHub Actions
[![Release](https://github.com/khulnasoft/go-vulncheck-action/workflows/Release/badge.svg)](https://github.com/khulnasoft/go-vulncheck-action/actions/workflows/release.yml)

Using [govulncheck](https://go.dev/blog/vuln)

## Usage

```yaml
name: govulncheck
on: [push]
jobs:
  test:
    runs-on: ubuntu-latest
    permissions:
      contents: read
    steps:
    - uses: actions/checkout@v3
    - uses: khulnasoft/govulncheck-action@v1
```
