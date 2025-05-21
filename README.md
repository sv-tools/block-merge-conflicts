# block-merge-conflicts

Check the changed files and block a Pull Request if the merge conflict markers are found.

The action uses GitHub API to get the list of changed files.

## Inputs

### `token`

**Required** GitHub Token.

## Example

```yaml
- uses: actions/checkout@v3
- uses: sv-tools/block-merge-conflicts@v1
  with:
    token: ${{ secrets.GITHUB_TOKEN }}
```
