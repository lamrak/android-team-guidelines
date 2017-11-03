### General rules before merging code:
1. You don't check in until it has been reviewed by someone else.
1. You don’t check in without adding tests, passing tests, or being verified (usually by CI).
1. You don't check in before reviewers complete and give the ":+1:".

***

### Pre code review:
1. Break large changes into smaller, more review-friendly pieces, with larger requests, it's too easy to miss something.
1. Don't split up changes if they are one cohesive change even if it is large.
1. Push unrelated bug fixes to your branch as separate commits, or as a separate commit on a new branch.
1. Double check if missed any test cases.
1. Send out code review after passing tests, but in case you get stuck or need help, start a PR(pull request) in the early stage with a label or comment stating that you need help.
1. Don’t avoid code review for trivial changes, should avoid the slippery slope of declaring changes to be "trivial" when they are not.
1. Using collaborative tools for reviewing code, eg.use the pull feature in github, don’t set up separate group discussion or do pair reviewing unless for a large change/feature.
1. As code is public, and more potential contributors will look at the code, it needs to be easily approachable to new developers, please add clear comments.
1. If you're fixing an issue that's listed in the github issue tracker or JIRA, reference the issue number in the commit message.
1. Code review is one of the most cost-effective methods of finding bugs, explaining well in objective and commit message is essential (why need the change, what is fixed, how it works).

***

### During code review:
1. You can optionally label the pull request with "needs review". This way the reviewer knows this pull request is finally ready to be reviewed.
1. Don't let code reviews slow you down, understand the tradeoff between the need to move quickly and the need to do things right, possible ways: respond their comments asap, make code easy to read, put clear comment, follow up with reviewer periodically, sending specific expectations to each reviewer, etc.
1. Create separate stories if possible so you can move forward with current work.
1. While it may seem more effective to cast a wide net to find a reviewer by requesting an entire mailing list or large sub-group to review a change, it actually tends to reduce the response rate, looking for right reviewers will be effective.
1. Follow up with the reviewers' status if no update for few days.
1. Notify reviewers about any changes during coding review.
1. If something in your code is not immediately clear to the reviewer, that is a good indication that a comment is required.
1. Don't squash the commits until it's ready to merge, squash may lose the comments from code review.
1. Don't forget to use a thumbs up emoji to indicate that you are done with the PR review.
1. Tests need to be part of the code review as well (unit test, functional test).
1. Reply every comment to prevent last minute change.
1. Finding a reviewer who cares about the particular area of the change is important and will generally lead to faster and more helpful reviews.
1. If reviewer can't review soon, let the submitter know.
1. If you requested multiple reviewers, make it clear what the expectations from each reviewer, either noting the expectation in the review request, or contacting them through some other channels or methods, e.g. use the @mention someone by their github handle, or email the reviewer.
1. To find a reviewer who is the owner of the code, or familiar with the code:
  Look at the authors that have recently modified a file.
  Find the last person to change related lines, using the git blame command.
  One other common place to look is the AUTHORS or README files within a project.

***

### Post code review:

***

### Checklist:
**Common issues:**

1. Does it follow the coding styles of the global development guidelines
1. Does it reinvent the wheel
1. Does it cover edge cases.
1. Does it meet the coding standards set for the appropriate language
1. Did the CI build pass.
1. Are all code paths tested.
1. Typos.
1. Clear comments.
1. Is it documented.
1. Error Handling, [When you must fail, fail noisily and as soon as possible.],
1. Is it giving reasonable amount of logging
1. Does it work on a different platform.
1. Is the error message informative.
1. Are there hard-coded data.
1. Is the program sufficiently modular.
1. Is all of the functionality necessary, could parts be removed without changing whole functionality.
1. Could the code be rewritten so that the comments aren't necessary.
1. Are variable names reasonable and self explanatory.

**Security issues:**

1.  Any passwords or secret keys stored within the source-controlled code or configuration files is not supposed.
1.  Is any logging of sensitive information
