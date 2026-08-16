#commands
- git clone -> clones the repo locally
- git remote -v ->displays the link to the remote repository

> we can have help on command line using git<command> -h
- e.g -> git clone -h , git remote -h

## commit
- A set of saved repository changes
- A commit is never lost
- A commit has a  hash key
- A commit is always the same

## stage and unstage
- git add <filename> = for staging
- git reset <filename> = for unstaging


# Branch
- git branch -> shows all the branches
- git branch <branchname> -> creates a branch
- git push -u origin <featureBranch>

# undo changes
- git revert<commit hash> -> creates a new commit that undoes the changes of the previous commit
- git reset <commit hash> -> it is default => git reset --soft
- git reset --soft<hash>  -> removes commits from history but keep the changes
- git reset --hard<hash>  -> removes the commits from history and removes changes

# Miscellaneous
- git push -f -> push forcefully from local to the remote one
- git push -> push to central repo from our local repo
- git pull -> allows us to retrieve the commits form central repository to our local project
- git log -> shows the log of a branch
- git show<commit hash> -> gives all the changes in all the file , including new file creation and yada yada in that commit
- git show <commit hash> --name-only -> will show only the filenames changed during that commit not the whole overwhelming info
- git reflog -> this commands show all the history and activity we did , including changing the branch and also shorthand hashkey,so that we can use
- git show for more detailed info of that commit
e.g
/*
❯ git reflog
607612b (HEAD -> main) HEAD@{0}: checkout: moving from featureBranch to main
7480c00 (featureBranch) HEAD@{1}: commit: feature branch commit
929b210 HEAD@{2}: checkout: moving from main to featureBranch
607612b (HEAD -> main) HEAD@{3}: commit: master branch commit
929b210 HEAD@{4}: checkout: moving from featureBranch to main
929b210 HEAD@{5}: checkout: moving from main to featureBranch
929b210 HEAD@{6}: commit (initial): first commit
*/
