#### Working with branches
----

Remember that new branches should be created off of the `staging` branch. 

Occasionally, you should make sure that you have the most-up-to-date `staging` branch within your fork by running the following commands:

```
git fetch upstream
git checkout staging
git merge upstream/staging
```

You should always be working inside a branch while solving an issue.

Make commits within the branch, and then -- when you're ready, push up the branch:

`git push --set-upstream origin BRANCHNAME` 

#### How to see a list of all existing branches
Type `git branch -a` to see a list of all available branches.

#### Switching branches
If you want to switch to an already-created branch, you would type `git checkout BRANCHNAME`. 

#### How to create a new branch
`git checkout -b BRANCHNAME`

Remember that our convention is to name the branch after the issue number we're working on.