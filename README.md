# Devbox for multiple teams with their own configurations
Team A: `devbox shell --config ./team-a/devbox.json`

Team B: `devbox shell --config ./team-b/devbox.json`

On CI: `devbox shell --config ./ci/devbox.json`

A shared plugin with packages, `init_hook`, scripts, etc is available in `./shared/plugin.json`

**Note**: On CI, Devbox loads packages based on the order you specify plugins in the `include` array. If you want any package, `init_hook`, or script specifically for the CI environment, add it to `./ci/devbox.json`.
