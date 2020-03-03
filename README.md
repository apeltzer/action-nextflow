# Nextflow GitHub Action

A simple Github Action to install a specific version of [`nextflow`](https://www.nextflow.io/).

## Usage

```bash
name: Test

on:
  push:
    branches:
      - master

jobs:
  test:
    runs-on: ubuntu-latest
    steps:
    - uses: apeltzer/action-nextflow@master
      with:
        version: 19.10.0
    - run: nextflow info

```
