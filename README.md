# Git notes

This repository is created with my goal to remeber some command by git.

## Commands:

### git rebase
this is an important commant but be carefull about it uses, normally this command
 is used to fix something in local environment.


Is important mention if it command is used in remote branch or main branch (master, steging, dev...) we could remove the correct commit history (branch), in other way we can change the order of commits

when we need to use this comman is important to follow the bellow steps:

* localizate in auxiliar branch (to remove) tect the comman mention to another branch (important branch)

`git rebase main`

* later that we can use git merge continue and fix the conficts.

*change the branch to important branch and repeat this proces

`git rebase aux_branch`


### git stash

It command is very util when we need to save a change without push, for example:
we have changes in branch *aux_brach* and we need to pass to main but in my current branch (aux_branch) i have some files edited so the wise to save my change and memory with stash

`git stash`

### git clean

git clean is a command that remove things that it can index (files) and is necessary taht they files are no in .gitignore, because in this case no is index by **git**

`git clean --dry-run`

### git cherry-pick

It is a method to select some special commit and moves it or extracts it to another branch.

Caution: when return our changes with merge it will create a confict

### git reflog
It shows all history in git without important if the branch, file was removed

### git reset --hard/--soft  #commit/HEAD@{5}
This command is dangerous because change the history of git.

--soft: maniant your changes in stash and you can return to especific commit 

--hard: return and remove all
