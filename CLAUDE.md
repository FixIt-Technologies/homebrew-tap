# FixIt Technologies Homebrew Tap

This private repository distributes signed-off release artifacts from FixIt
Technologies projects through Homebrew.

- Casks are generated and published by upstream GoReleaser pipelines.
- Never put release binaries or credentials in this repository.
- Human changes use pull requests. A repository-scoped deploy key may update
  generated casks directly after a successful upstream release.
- Private-release casks must defer `HOMEBREW_GITHUB_API_TOKEN` lookup to their
  download strategy; Homebrew scrubs sensitive variables while loading casks.
