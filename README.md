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
