'git init' -> Powers your folder to be managed by git ,and initialises a new empty repository
. It also creates a .git folder tht has all the relevant logic to manage versions 
of your project.

2. 'Working Area' -> There can be a bunch of files that are not currently Handled by git.
It means that changes done or to be done on those files are not manage by git yet.A file
which is in working area is considered to be not in the staging area. When we do 'git status' 
and we see a bunch of 'untracked files' then these are actually called to be in the working area.

3. 'Staging Area' -> What all files are going to part of the next version that we will create.
This staging area is the place where git knows what chnages will be done from the last version 
to the next version.

4. 'Repository Area' -> This area actually contains the details of your registered version .
And the files in this area ,git already manages them and knows there version history.

5. 'git add <files>' -> moves file working area to staging area.

6. 'git rm --cached <files>' -> This moves from file back from staging area to working area.

7. 'commit' -> Commit is a particular version of the project. It captures a snapshot of the project's staged 
changes and creates a version out of it.

8. 'git commit' -> registers staging changes to a commit.

9. 'git log' -> list down all the commits of the repository.If you want ot out of git 
log prompt press 'q'.

10. 'git restore <files>' -> it removes all files changes from the starting area to be commited.
this can be useful, if we did some dirty piece of code and now no more want it. Instead of deleting every change
line by line .we can restore it you can say restore last clean version of the file.

11. 'git restore --staged <file>' -> it removes file changes from staging area to the working are.
This only works if changes are in your staging area.

12. Diff between git rm and git restore 
ans: if you want to move the whole file bck to the untracked state, then we do git rm,otherwise if we just
want the changes to be moved in working area or staging area then we use git restore.

13. 'git diff commit1 commit2' -> gives the difference of all file change between two commits.

14. 'git commit -m "" ' -> If we want to be avoid opening a text editor like vim/nano to add commit message we can use this following command.

15. 'git remote' -> list down all the remote connection names

16. Remote connection -> It helps you to link two git repositories for upoading and downloading changes
from each otherwise.

17.'git remove add <name of remote> <link of the remote>' ->this command helps us to add new link to the remote repo
and give a name to it.

18. 'give remote rm <name of remote>' -> this command deletes a remote connection.

19. 'git remote rename <oldname> <newname>' -> this command renames the emote connection.

Note: The name of the remote connection is always used to establish communication between the repos.

20. 'git pull <remote name><branch name> : downloads latest chages from the branch of the mentioned remote in your local repos.

#### Recommended practise ####
- make changes
- git add <files>
- git commit
- git pull
- git push

