# Don't Run on Draft PR

This GitHub Action will fail if the Pull Request is a draft. The idea is adapted from [this discussion](https://github.com/orgs/community/discussions/25722#discussioncomment-3248921).

## Example

```yaml
jobs:
  dont-run-on-draft-pr:
    name: Don't Run on Draft PR
    runs-on: ubuntu-latest
    steps:
      - uses: z0gSh1u/dont-run-on-draft-pr@v1

  whatever-else:
    needs: dont-run-on-draft-pr
```

Let's see if it works...
