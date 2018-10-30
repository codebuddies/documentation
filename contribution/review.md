#### Reviewing Pull Requests
----

Yes, you can help review PRs! If you're interested in helping review a [submitted PR](https://github.com/codebuddies/codebuddies/pulls), just follow the simple steps below to get started.

1. Add the contributor's forked repo to your remote:

    `git remote add <contributor> https://github.com/<contributor>/codebuddies.git`

2. Fetch the date from the contributor's forked repo:

    `git fetch contributor`

    **N.B:** `fetch` is only used when you want to check out a PR from a forked repo.

3. Switch to the relevant branch in the contributor's repository:

    `git checkout contributor/<name of branch>`
    
    You can find the name of the branch you need to check out at the bottom of the PR submitted by the contributor. 

When you start up the app again on your machine (`meteor --settings settings-development.json`), you will see the relevant PR submitted from the contributor's forked repo running on localhost in your browser.
