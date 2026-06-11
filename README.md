# team-ai-sync demo source

This public repository is the source of truth for a working
[`team-ai-sync`](https://github.com/paladini/team-ai-sync) demonstration.

It models a team that wants to keep AI collaboration files aligned across an API
repository and a web repository without copying files by hand.

## Repositories in this demo

- [team-ai-sync](https://github.com/paladini/team-ai-sync) provides the GitHub
  Action used by this demo.
- [team-ai-sync-demo-source](https://github.com/paladini/team-ai-sync-demo-source)
  stores the shared files, `sync-config.json`, and workflow.
- [team-ai-sync-demo-api](https://github.com/paladini/team-ai-sync-demo-api)
  receives the generated API sync pull request.
- [team-ai-sync-demo-web](https://github.com/paladini/team-ai-sync-demo-web)
  receives the generated web sync pull request.

## Demo flow

1. Update shared guidance in this repository.
2. Run the
   [Sync AI Assets workflow](https://github.com/paladini/team-ai-sync-demo-source/actions/workflows/sync-ai-assets.yml).
3. Review the generated pull requests in the target repositories:
   - [API demo pull request](https://github.com/paladini/team-ai-sync-demo-api/pull/1)
   - [Web demo pull request](https://github.com/paladini/team-ai-sync-demo-web/pull/1)

The workflow first supports a `dry-run` input so the sync can be demonstrated
without creating branches or pull requests.

## Evidence

- [Dry run with changes detected](https://github.com/paladini/team-ai-sync-demo-source/actions/runs/27315787215)
- [Real sync run that created pull requests](https://github.com/paladini/team-ai-sync-demo-source/actions/runs/27315807029)
- [Update run that reused existing pull requests](https://github.com/paladini/team-ai-sync-demo-source/actions/runs/27315999623)
- [Final dry run with no changes](https://github.com/paladini/team-ai-sync-demo-source/actions/runs/27316035674)
