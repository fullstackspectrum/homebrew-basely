[![Basely: a better base image, with the evidence.](https://raw.githubusercontent.com/fullstackspectrum/basely/main/docs/brand/readme-banner.png)](https://github.com/fullstackspectrum/basely)

# Homebrew tap for Basely

The Homebrew formula for [Basely](https://github.com/fullstackspectrum/basely), which compares each `FROM` in a Dockerfile with slim, hardened, Chainguard and newer-runtime images on vulnerabilities, size and fit, and recommends a better one.

## Install

```bash
brew install fullstackspectrum/basely/basely
```

That taps this repository and installs Basely in one step. Basely runs on Homebrew's Python 3.14, which reads the zstd-compressed layers Docker Hardened Images use.

## Upgrade

```bash
brew upgrade basely
```

## Try it

```bash
basely advise                      # reads ./Dockerfile
basely compare python:3.12 python:3.12-slim dhi.io/python:3.12
```

See the [Basely README](https://github.com/fullstackspectrum/basely#readme) for every option, the GitHub Action and the container image.

## About this tap

`Formula/basely.rb` is generated. Each Basely release renders it from [`packaging/homebrew/basely.rb`](https://github.com/fullstackspectrum/basely/blob/main/packaging/homebrew/basely.rb) with the release's source distribution on PyPI and pushes it here. Change the template in the Basely repository rather than editing the formula in this one.

Issues with Basely itself, or with installing it, go to [fullstackspectrum/basely](https://github.com/fullstackspectrum/basely/issues).

Basely is part of [Full-Stack-Spectrum](https://fullstackspectrum.com/).
