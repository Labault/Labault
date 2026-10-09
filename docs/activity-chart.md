# Activity chart

The profile embeds static SVGs from this repository. A failed refresh leaves the
last successful charts available, without depending on a live image service.

[Deus Commit Chart](https://github.com/dturovskiy/deus-commit-chart) generates a
90-day contribution curve and a seven-day moving average. Contributions follow
GitHub’s calendar rules; they are not a count of commits alone. The README uses
`<picture>` to select the native light or dark theme.

## Refresh

The [workflow](../.github/workflows/activity-chart.yml) runs daily at 03:17 UTC,
when its configuration changes on `main`, or through **Actions → Update activity
chart → Run workflow**. Scheduled runs can be delayed by GitHub.

Only `assets/activity/activity-dark.svg` and `activity-light.svg` are committed.
Both themes must generate successfully before publication. The job commits to the
default branch only when the SVGs change, without force-pushing. Refresh commits
do not trigger another run.

The workflow needs permission to push to the default branch. Branch protection
may prevent that; in that case, download or regenerate the charts and update them
through a pull request.

## Contribution visibility

The default token is the workflow’s `GITHUB_TOKEN`. To request private contribution
counts, optionally set the repository secret `ACTIVITY_GRAPH_TOKEN` to a dedicated
token with the necessary read access. Keep it in Actions secrets.

The result depends on the token’s access and your profile’s private-contribution
settings. Only aggregate daily counts are published, with no repository names or
commit details. Initial SVGs were generated locally using the authenticated GitHub
CLI; the workflow’s default token may return a different contribution count.

## Dependencies

Checkout and the chart generator are pinned to commit hashes. When updating the
generator, check its inputs, regenerate both themes and inspect the SVGs before
changing the pins. The upstream composite action manages its own Node.js runtime.
