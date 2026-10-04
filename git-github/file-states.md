# Git file states

Git has multiple file states, depending on the area where these are currently in.

- **Untracked** Is the state where the changes inside a file are not being tracked by Git.
Commonly happens with newly created files.

- **Modified** Is when a file that is already being tracked gets modified.

- **Staged** Is when the modifications of a file are sent to the staging area to be commited.

- **Commited** Is the state where the changes are made and a commit is created along side the changes.

## Flow of the states

We can visualize it as follows:

```
file.txt -> [Untracked] -> git add file.txt ->
[Staged] -> git commit -m "added file.txt" -> [Commited]
```

