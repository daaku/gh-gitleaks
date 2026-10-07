# gh-gitleaks

A simpler less featureful approach to running gitleaks.

```yaml
steps:
  - uses: daaku/gh-gitleaks@main
```

Pin a specific version if you like; without it the latest release is used.

```yaml
steps:
  - uses: daaku/gh-gitleaks@main
    with:
      version: 8.30.1
```

The binary is cached with
[`actions/cache`](https://github.com/actions/cache) under the requested version
(or `latest`), so a warm cache is reused as-is, with no extra requests. It is
only downloaded on a cold cache.
