# Commit to remote with GitHub API

This is a work in progress GitHub action which uses the GitHub API's [Git Data endpoints][git-api] to commit all changes to a remote (defaults to master).

This will squash all changes into a single commit. Future plans include an option to preserve commit history.

Because this is using the GitHub API to create new commits, the SHA-1 hashes may differ. I'm not sure if that will work yet.

Using the GitHub API instead of `git push` like @ad-m's [GitHub Push][git-push-action] action allows this to work without requiring setup of a Personal Access Token.

[git-api]: https://developer.github.com/v3/git/
[git-push-action]: https://github.com/ad-m/github-push-action
[ad-m]: https://github.com/ad-m
