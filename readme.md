## Git Commands 

1. `git init` -> Power your folder to use git and initialize and empty git repository.It also creates a .git file which contains all the logic for managing the versions of your project.

2. `git add < filename >` -> Use this command to add a file to the staging area from the working. Note - To add all the files to the staging area use `git add .` .

3. `git rm --cached < filename >` -> Use this command to remove a file from staging area back to working area.

4. `commit` -> Commit is a particular version of the project. It captures a snapshot of the projects staged changes and creates a version out of it.

5. `git commit -m "Message"` -> Use this command to register staging changes to the commit.

6. `git log` -> Lists down all the commits in the repository.

7. `git restore < filename >` ->  It removes all the file changes from the working area which are to be staged. This can help in removing dirty piece of code.

8. `git restore --staged < filename >` -> It removes all the file changes from the staging area to the working area.

9. `git diff <commit id-1> <commit id-2>` -> Used to see the new changes added between two commits. You can get the commit id's using the `git log` command.

10. `git remote` -> Lists down all the remote connection names.

11. Remote connection -> It links two git repositories for uploading and downloading changes from each other.

12. `git remote add <name of remote> <link of remote>` -> This commands helps us to add a new link to the remote repo and gives a name to it. Ex- origin

13. `git remote rm <name of remote>` -> Deletes the remote connection.

14. `git remote rename <old-name><new-name>` -> This renames the remote connection.
Note - The name of the remote connection is always used to establish a connection between the two repos.

15. `git pull <remote name> <branch name>` -> Download latest changes from the branch of the mentioned remote


### Recommended Practice to do - 
      
      - make changes
      - git add <file>
      - git commit
      - git pull
      - git push


## Different Areas in Git

1. `Working area` -> Files which are not being currently handled by git are in the working area.It means changes done to these files are not managed by git. When on using the `git status` command if there are `untracked files` then these are the files currently in the working area.

2. `Staging area` -> Files in the staging area represent what all files are going to be the part of the next version. The staging area is the place were git knows what all changes are going to be done in the previous version to the next version.

3. `Repository area` -> This area contains all the details of the previously registered versions. Git knows and manages the version history of all the files in this area.

Difference between rm and restore
 - Ans - git rm is used to move back the entire file to an untracked state whereas git restore is used to move the files from working and staging area.

Merge conflicts are very common scenario.
