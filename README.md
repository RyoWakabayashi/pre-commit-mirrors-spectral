# spectral mirror

Mirror of spectral package for pre-commit.

For pre-commit: see <https://github.com/pre-commit/pre-commit>

For spectral: see <https://github.com/stoplightio/spectral>

## Using spectral with pre-commit

Add this as `.spectral.yaml`:

```yml
---
extends: spectral:oas
```

Then add this to your `.pre-commit-config.yaml`:

```yml
- repo: https://github.com/RyoWakabayashi/pre-commit-mirrors-spectral
  rev: "v6.4.0" # Use the sha / tag you want to point at
  hooks:
    - id: spectral
```
