# Git zones

Git works in 3 different zones: the _working tree_, the _staging area_, and the _commit_.

- **Working tree** Is the zone where all local files are stored. They are located in your CWD
(the one where the `.git` dir is located). Its purpose is to track all changes made to files.

- **Staging area** Is the zone where changes that are ready to be _commited_ are sent.

- **Commit** Is the final stage of a change. The changes sent to the staging area are saved and a 'snapshot'
(the commit) is created to track the changes made. It stores time, author, and content changed.

I lied, there are not only 3 zones in Git. Theres actually an extra zone (if we can consider it a zone). The stash.

- **Stash** Is a zone used to temporary store changes made in both the working tree and the staging area.
The stash works just like a stack data structure, the last stash will pop next and so on until its empty.

## See next

- [Git file states](file-states.md)
