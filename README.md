# Discussion Topic
https://github.com/renovatebot/renovate/discussions/24163

# Requirements
1. All recommended mono repos should have their PRs grouped by repo
2. All other packages should have their updates in separate PRs
3. Only match packages in `dependencies` & `devDependencies`
4. Ignore packages in `peerDependences`

# Expected Results
After running renovate, we would like to have a list of PRs similar to below:
- Update babel monorepo
- Update jest monorepo
- Update material-ui monorepo
- etc. (the rest of mono repos that match `group:monorepos` preset)
- Update classnames ^6.5.4 -> ^6.24.0
- Update debounce ^1.2.0 -> ^1.2.1
- Update chromatic ^6.5.4 -> ^6.24.0
- etc. (any remaining packages NOT belonging to any mono repos)
