# Devbox for multiple teams with their own configurations
Team A: `devbox shell --config ./team-a/devbox.json`

Team B: `devbox shell --config ./team-b/devbox.json`

A shared plugin with packages, `init_hook`, scripts, etc is available in `./shared/plugin.json`
