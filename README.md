# gh_merge_trigger

Test project for GitHub Actions workflow triggered by merging a PR with the "Build" label to the master branch.

## How it works

The workflow (`.github/workflows/build-on-merge.yml`) triggers when:
1. A pull request is closed on the `master` branch
2. The PR was actually merged (not just closed)
3. The PR has the label `Build`

## Testing the workflow

1. Create a new branch: `git checkout -b test-branch`
2. Make some changes and commit them
3. Push the branch to GitHub
4. Create a PR to merge into `master`
5. Add the `Build` label to the PR
6. Merge the PR
7. The workflow should trigger automatically

## Customizing the build

Edit the "Run build" step in `.github/workflows/build-on-merge.yml` to add your actual build commands.
## Test1

### Test2
### Test3
