If we want to just download the changes in a remote branch and not merge them automatically (as in the pull command) we could use the fetch command that does exactly that.
```git
git fetch origin main
```

This command will just download the changes, but won't apply them directly in the local repository. After that we can see the differences between the local repository and the remote repository that we just downloaded with the diff command:

```git
git diff main origin/main
```

With that, we are comparing the differences between the main branch and the main branch in origin, which belongs to the remote repository.