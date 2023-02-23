# isort-action

## How to use

```
jobs:
  codeformat:
    if: github.event_name == 'pull_request'
    runs-on: ubuntu-latest

    steps:
      - name: Check-out
        uses: actions/checkout@v3
        with:
          fetch-depth: 1

      - name: Poetry install
        uses: wintero92/poetry-install-action@v1

      - name: Isort
        uses: wintero92/isort-action@v1
```

## Inputs

See `action.yaml` for possible inputs.
