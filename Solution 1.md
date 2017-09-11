##Solution 1##
1. a. checkout allows you to go in to another branch and work there instead of the master. helps when you want to work on something and are worrying about messing something else up.

A working copy is a program or file that you are currently editing. 

A branch is part of a git where you can transfer information and work outside of the master. 

Update means to change the project into the most recent copy. This does not mean it has to be a working copy. You can use git pull or git merge.

A commit is used to explain what is being added into a repository - gives a log of information.

Pushing lets you push your changes to the repo and adds your commit. 

Pull updates your remote repo.This would be like taking files from an online repo like github and updating them on your system.

Clone allows you to create a remote repo. Cloning links up your system to the online repo.

b.  Git vs. Subversion - git is decentralized. This means that even if you do not have any internet, you can still commit and when you get internet, it will commit for you. You do not have this with subversion. You will have to copy and paste to make sure you are able to commit later. They are still used for the same reason though - to keep versions of previous versions and copies of things that have been done to the repo.

c. "Git pull" will update the working repository in git. "svn update" updates in subversion. 

d. When there is a conflict, this means that git doesnt know which file to change. A conflict could be.. the same feature is already updated on one repo and youre trying to send it again or the same feature is updated in one repo and deleted in another. You can undo a merge to fix a conflict. This can mean using the following command to undo a commit:
> git commit -m "fix the conflict"

> git reset HEAD~

> git add .

> git commit -c ORIG_HEAD

I got a merge conflict because i changed the conflict.cpp file and tried merge. I can't pull my information from the repo because i have unmerged files. You can see my conflict when you run git status. 
This gives me:


> On branch master


> Your branch and 'origin/master' have diverged,
and have 2 and 1 different commits each, respectively.
  

> (use "git pull" to merge the remote branch into yours)
You have unmerged paths.
  

> (fix conflicts and run "git commit")
  

> (use "git merge --abort" to abort the merge)



> Unmerged paths:
  (use "git add <file>..." to mark resolution)

        both modified:   conflict.cpp

(I tried the git mergetool and it didnt work. It added a few files but i can delete with the rm command. Instead I am using 

> git add conflict.cpp

The conflict is now resolved. 