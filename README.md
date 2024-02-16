﻿# conflict-test
This reository is about creating a new branch, creating merge conflicts and resolving merge conflicts

## Git Branching

To categorize the different functionalities of the project we create branches to keep organized. Later we merge these branches into master branch. 

## Fundamental principles:  

-> Whenever new branch is created up to that point entire commit history is copied into the new branch. After creating the commit       
   history is separated as per our commits into respective branches 
-> Git merge committed history happens based on timestamps while merging different branches.

## To merge the branch :  

First checkout to the respective branch that we want to be merged 

Give command ```git merge <branchname>```

##  To create new branch
```
git branch  <branch name>
```
## To create new branch and to move into that branch
```
git checkout –b  <branch name>
```

## Git pull vs git fetch 

Git fetch: git fetch downloads only the modified code and places that code in the separate branch called remote branch so that I can go to that branch and check if modifications are ok then we can merge it otherwise  we  leave it 

-> This will help in resolving conflicts  

Git pull: Git pull downloads the modified code places into our branch directly without our permission by merging it 

-> This will help in pull the code from remote to our local branch such that this is very certain that code is no conflicts 

 
Git rebase : 

Whenever we want to project latest code or modified code we use "git rebase master". This will make the test branch committed history to sit at the top of master branch history. 

Git rebase  command : ```git rebase <branch name> ```

