# git
Git Command

Change to local git repository

```cd <repo_name>```

List all branches

```git branch -a```

You should see something similar to the following:

``` 
* master   <feature_branch>
  remotes/origin/<feature_branch>
  remotes/origin/master
```
Notice that it lists both the branches that are local and the remote branches on Bitbucket. Using the list as reference, choose the branch you want to checkout.  In this example, the feature branch is the branch.

Checkout the branch you want to use.
```
git checkout <feature_branch>
```

Confirm you are now working on that branch:
```
git branch
```
You should see something similar to the following:
```
* <feature_branch>
  master
```
Going forward, all your Git commands apply to the branch.  When you push the changes to your remote Bitbucket repository, those changes apply to the repository's branch.

you can delete branch -d option
```
git branch -d <feature_branch>
```
git 
https://confluence.atlassian.com/bitbucket/branching-a-repository-223217999.html
https://git-scm.com/book/en/v2/Git-Branching-Basic-Branching-and-Merging

READMe document
https://help.github.com/articles/basic-writing-and-formatting-syntax/


Step 1. Fetch and check out the branch for this merge request

```git fetch origin
git checkout -b login-page origin/login-page
````

Step 2. Review the changes locally

Step 3. Merge the branch and fix any conflicts that come up

```git checkout master
git merge --no-ff login-page
```

Step 4. Push the result of the merge to GitLab

```git push origin master
```

