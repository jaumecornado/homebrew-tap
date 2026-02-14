# Homebrew Tap

Official Homebrew tap repository for custom CLI tools and packages.

## Add This Tap

```bash
brew tap jaumecornado/tap
```

## Install a Formula

```bash
brew install <formula-name>
```

Example:

```bash
brew install holded
```

## Upgrade Installed Formulae

```bash
brew update
brew upgrade
```

## Publish Formulae to This Tap

Each source project can publish/update its formula in this tap (for example via
GoReleaser on tag pushes).

Required environment variables or GitHub Actions secrets in each source project:

- `HOMEBREW_TAP_OWNER=jaumecornado`
- `HOMEBREW_TAP_NAME=homebrew-tap`
- `HOMEBREW_TAP_GITHUB_TOKEN=<PAT with write access to this tap repo>`

With these configured, releases can publish binaries + checksums and commit formula
updates into `Formula/*.rb` in this repository.
