# team-ai-sync demo source

This public repository is the source of truth for a `team-ai-sync` demonstration.

It models a team that wants to keep AI collaboration files aligned across an API
repository and a web repository without copying files by hand.

## Demo flow

1. Update shared guidance in this repository.
2. Run the `Sync AI Assets` workflow.
3. Review the generated pull requests in the target repositories:
   - `paladini/team-ai-sync-demo-api`
   - `paladini/team-ai-sync-demo-web`

The workflow first supports a `dry-run` input so the sync can be demonstrated
without creating branches or pull requests.
