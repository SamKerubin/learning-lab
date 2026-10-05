# Merge conflict

When merging a branch, it is possible encountering conflicting changes.
These conflicting changes happen when a file is modified in 2 different branches,
making Git confused about which version is the correct version.

To solve these conflicts, one first needs to identify where and what is conflicting,
then we need to manually decide whether our changes stay or not.

Conveniently, Git modifies the file being in conflict, making it look like this:

```
<<<<<<< HEAD
changes-in-main
=======
changes-in-branch-1
>>>>>>> branch-1
```

`<<<<<<<`, `=======`, `>>>>>>>` work as markers. They indicate where both changes come from.
