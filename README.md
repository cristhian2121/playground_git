### Git notes

This repository is created with my goal to remeber some command by git.

### Commands:

#### git rebase
this is an important commant but be carefull about it uses, normally this command
 is used to fix something in local environment.


Is important mention if it command is used in remote branch or main branch (master, steging, dev...) we could remove the correct commit history (branch), in other way we can change the order of commits

when we need to use this comman is important to follow the bellow steps:

* localizate in auxiliar branch (to remove) tect the comman mention to another branch (important branch)

`git rebase main`

* later that we can use git merge continue and fix the conficts.

*change the branch to important branch and repeat this proces

`git rebase aux_branch`


#### git stash

It command is very util when we need to save a change without push, for example
