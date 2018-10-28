#### Reviewing pull requests
----

Love to make a review on a [submitted PR](https://github.com/codebuddies/codebuddies/pulls)? Just follow the simple steps below to get started.

1. Add the contributor's forked repo to your remote:

    `git remote add <contributor> https://github.com/<contributor>/codebuddies.git`

2. Fetch the date from the contributor's forked repo:

    `git fetch contributor`

    **N.B:** `fetch` is only used when you want to check out a PR from a forked repo.

3. Switch to the name of the remote you used(in this case, contributor):

    `git checkout contributor`

When you run the server on your machine, you should see the version of the contributor's forked repo running on localhost in the browser.