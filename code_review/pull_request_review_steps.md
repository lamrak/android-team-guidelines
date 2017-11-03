## PR Author

1. Push your changes into separate branch like `feature/user-login`.
1. Create Pull Request with `develop` as base branch and you branch from step 1.
1. Write proper and meaningfull description of the purpose of this PR.
1. Put label <kbd>[Status: In Progress]()</kbd> on the PR.
1. If your PR is ready to be reviews remove <kbd>[Status: In Progress]()</kbd> label and put <kbd>[Status: Review Needed]()</kbd>.
1. Assign a reviewer for the PR.
1. After PR gets approved by reviewer and it has label <kbd>[Status: Mergeable]()</kbd> you can merge it and delete feature branch.
1. If not, remove <kbd>[Status: Changes Requested]()</kbd> label and add label <kbd>[Status: In Progress]()</kbd> and start working on it.
1. After pushing fix commits add proper commets to the reviewer's commets like:
```Whoops. Good catch, thanks. Fixed in a4994ec.``` 
1. When all requested changes are fixed remove label <kbd>[Status: In Progress]()</kbd> and add <kbd>[Status: Review Needed]()</kbd>.

## PR Reviewer

1. If everything is OK with code - approve changes and replace <kbd>[Status: Review Needed]()</kbd> label with <kbd>[Status: Mergeable]()</kbd> label.
1. When an issue is found - write proper comments and link to the code where it was found.
1. When all found issues have proper comments, please change label to <kbd>[Status: Changes Requested]()</kbd>
1. When you are done with review write someting inspiring to the author in PR comment like :thumbsup: .
