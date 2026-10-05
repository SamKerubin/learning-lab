# Rebasing

Rebasing is an alternative way of merging branches.
Its purpose is to reatach the commits made in a branch to the HEAD of main.

Rebasing should never be done in public branches, only inside local branches.
This is because rebase can alter and modify the commit history of the repository.

## Visualization

```
-- before rebase

    
        o - o <- (branch-1)
      /
o - o - o - o <- (HEAD)


-- after rebase

              o - o <- (HEAD)
             /       
o - o - o - o

```

Its honestly a bit easy mistaking rebase with fast-forward.
The key difference between both is that rebase reataches the commits to HEAD
even if the main branch has suffered any changes, while fast-forward only happens
when no changes were made.
