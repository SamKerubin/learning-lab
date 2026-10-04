# Guide on how to setup a remote repository on GitHub

1. Open your terminal
2. Execute `git init .` to create the `.git` directory inside the CWD.
3. Make a commit, you can create a `README.md` as a placeholder to make the inital commit.
4. This can be splitted into 2 sections, with the same results:

    4.1. If you are going to host the repository, go to you GitHub and create one.
    4.2. If you are trying to get access to another repository,
    first make sure you have enough permissions as a collaborator and simply type
    `git remote add <name> <url>`, usually replacing 'name' with 'origin' and 'url'
    with the complete url of the repository.

5. Finally, you just push your changes to the main branch.

## Example

```bash
git init .

## make any change

git add .

git commit -m "Initial commit"

git brach -M main # ensure the default branch is main, optional but really recommended

                        # dummy url (this repository url)
git remote add origin "git@github.com:SamKerubin/learning-lab.git" # <- you can always find this url inside your GitHub copy

git push -u origin main # we use -u here so we can push directly to main on future commits. its also optional

```

And thats it! You created a remote repository on GitHub.
