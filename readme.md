# gh-gitleaks

A simpler less featureful approach to running gitleaks.

```yaml
steps:
  - uses: daaku/gh-gitleaks@main
```

The gitleaks binary is cached with
[`actions/cache`](https://github.com/actions/cache), keyed on the latest release
version, so it is only downloaded when a new version comes out.
