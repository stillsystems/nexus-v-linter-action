# Nexus-V Linter Action

[![CI](https://github.com/stillsystems/nexus-v-linter-action/actions/workflows/ci.yml/badge.svg)](https://github.com/stillsystems/nexus-v-linter-action/actions/workflows/ci.yml)

Automated validation and linting for **Nexus-V** templates. This action ensures that your template repositories adhere to the Still Systems standards and have valid metadata.

## Usage

Add this to your `.github/workflows/lint.yml`:

```yaml
name: Lint Template

on: [push, pull_request]

jobs:
  lint:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - uses: stillsystems/nexus-v-linter-action@main
        with:
          path: '.'
```

## Inputs

| Input | Description | Default |
|-------|-------------|---------|
| `path` | Path to the template directory | `.` |
| `version` | Nexus-V version to use | `latest` |

---
🧱 **Still Systems** — Tools engineered for real-world conditions.
