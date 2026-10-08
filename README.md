# fork-sync

Scheduled GitHub Action that syncs every fork owned by this account with its upstream every 4 hours (`.github/workflows/sync-forks.yml`).

- Secret `FORK_SYNC_TOKEN`: a github.com token with `repo` and `workflow` scopes (`workflow` is needed when upstream changes workflow files).
- Run it now: `gh workflow run sync-forks -R nareshh74/fork-sync`.
- GitHub disables scheduled workflows after 60 days without repository activity. Re-enable it from the Actions tab, or push any commit.
