The reset command will be necessary when we want to delete a wrong done commit.
There is three arguments that we can use with this command, each providing divergent results that are useful to different situations:
- soft
- mixed
- hard

The structure of the command is as follows:
```git
git reset --argument <commit hash>
```

In the argument we use one of the three and in commit hash we use the hash of the commit to which we want to return, removing the later ones.

##### Soft
Using the reset command with the soft argument, removes the commits and move the files to the stage area, so we can commit again as is, or add more changes.

##### Mixed
The mixed argument removes the commits and leave the files only in the repository, so we have to manually add them again as we want

##### Hard
The hard argument removes the commits and also removes the files and changes from the later commits from the repository, so think well before using it.

### Removing Selectively
Sometimes it is not mandatory to reset an entire commit, so in that case, we can reset only selected files using the same command, but passing the file path:

```git
git reset <filepath>
```