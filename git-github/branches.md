# Git branches

Git works in a system based off 'branches'. Branches are lines of work where commits are stored in chronological order.

The default branch Git uses is usually called 'main' (we call it the main branch).
Other branches different from main are paralell lines working around main.

Branches different from main have one purpose: make changes without modifying main directly.
Then merge that branch into main to apply all the changes.

There are 2 types of merging in branches:

- **Fast-forward** Happens when the main branch hasnt suffered any changes since the creation of the branch.
Merging these changes is as simple as moving the HEAD pointer to the top of the branch (immediately making it part of the main branch).

- **Merge** However, happens when changes were made in the main branch (or if it was forced with `--no-ff`).
Git will create a new commit merging the changes made in both branch, a merge commit.

## Visualization

### Fast-forward

```
-- before merge

  (HEAD)
    |
    |   o - o <- (branch-1)
    v /
o - o 


-- after merge

        o - o <- (HEAD)
      /
o - o 

```

### Merge

```
-- before merge

    
        o - o <- (branch-1)
      /
o - o - o - o <- (HEAD)


-- after merge

    
        o - o <- (branch-1)
      /       \
o - o - o - o - o <- (HEAD)

```

* Note that fast-forward will automatically delete the branch, while merge keeps the branch alive

## See next

-  _[Rebasing](rebasing.md)_
