# Make the current commit the only (initial) commit in a Git repository

**Description :**   Deleting the .git folder may cause problems in your git repository. If you want to delete all your commit history but keep the code in its current state, it is very safe to do it as in the following:

**Example** :

```powershell
iwr -useb get.scoop.sh | iex
git config --global credential.helper manager-core
scoop install sudo
scoop install windows-terminal
scoop install extras/vcredist2022
scoop install starship
scoop install fzf

```


**this will not keep your old commit history around**


**[based on a mix of answers in stackoverflow](https://stackoverflow.com/questions/9683279/make-the-current-commit-the-only-initial-commit-in-a-git-repository)**
