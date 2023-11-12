# java-maven

# Workflow

**Workflow file:** [ci.yml](.github/workflows/ci.yml)

**Description:** Build and run tests.

## Input parameters

| Name         | Description | Required | Type   | Default |
| ------------ | ----------- | -------- | ------ | ------- |
| java-version | JDK version | false    | string | 17      |

## Output parameters

None

## Workflow usage example

```yaml
name: main

on:
  push:
    branches: ["main"]
  pull_request:
    branches: ["main"]

jobs:
  ci:
    uses: repo-meister-actions/java-maven/.github/workflows/ci.yml@main
```

## Repositories using this workflow

- [robvanderleek/JLifx](https://github.com/robvanderleek/JLifx/blob/main/.github/workflows/main.yml)
