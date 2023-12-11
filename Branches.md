When working in a team or with multiple features simultaneously it can be very difficult, as different files are going to be commited without a clear order. In those cases, conflicts can happen. Or maybe we just want to test something without affecting the main program.
In those cases the Git branches can be very helpful. They work as a pointer, pointing to an specific commit, and with them we can separate features, teams, version and more.
In the terminal we can create a branch with the following command:
```git
git checkout -b <new-branch-name>
```

And we can change the current working branch with the same command but without the argument "-b"
```git
git checkout <branch-name>
```

#### Listing Branches

We can see all the project branches with the branch command:
```git
git branch
```

We can see which commit each branch points to with the "-v" argument:
```git
git branch -v
```


#### Merging Branches
In the case that we have gone through all the required tests and the feature we were developing in the branch works well, we now want to transfer all the changes to the main branch. For that we enter the main branch and use the merge command:

```git
git merge <branch-to-merge>
```


#### Deleting Branches
After making the tests we wanted, or after merging the test branch to the main branch, we might not want this branch to exist anymore, so we can delete it with the "-d" argument:
```git
git branch -d <branch-to-delete>
```

#### Downloading a single branch from a remote repository
In the case we want a specific branch from a repository we can use the [[Git Clone|clone]] command but informing git which branch we want to clone and also inform that it is the only branch the we wish to clone:
```git
git clone https://github.com/User/Repository.git --branch <branch-name> --single-branch
```