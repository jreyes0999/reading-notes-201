# Git Tutorial

## Version Control (VCS)
  * Allows you to revisit different version of a file or files by recording changes. You can then track changes, modify certain files, and even compare changee, which helps you revise for mistakes.
## Local Version 
  * A database on your hard drive stores file changes. 
## Centralized Version Control (CVCS)
  * A single server hosts all the changes and different versions of the files and other users can access those files 
## Distributed Version Control (DVCS)
  * Fixes the weakness of a CVS, if the CVS fails, then you will be unable to reach those files and their different version. A DVCS allows for users to create mirror repositories in case of the server going down to replace any information that gets lost. 

# So what is Git? 
## Git Features 
  * Git is a DVCS that stores data in a file system made up of snapshots. Each time you save a changed version of your project — called commit — Git creates a snapshot of the file and stores a reference to it. If the file has not changed, Git only stores a reference to the already-stored identical version of it.
  * Git relies on local operations, meaning it is on the users computer/local disk so it doesn't have to fetch anything from the servers and allows you to work on it even when you're offline or on a VPN. 
  * Git always trakcs any change applied to a file or director and it will detect file corruiption or information loss, but Git makes it's very difficult for these things to happen to any committed files. 
  * There are 3 different states of a file: Committed, modified, and staged. Committed means the data is securely stores in a local database, modified means a file has been changed, but it hasn't been committed yet, and stages means a file is flagged as a changed version and will update in the next commit. 
## Local Repository Structure
  * The local Git repository has three components:
    * Working Directory: The actual files reside here.
    * Index: The area used for staging
    * Head: Points to the most recent commit
**All files in a checked out (or working) copy of a project file are either in a tracked or untracked state**
  * **_Tracked_** - Tracked files can be modified, unmodified, or staged; they were part of the most recent file snapshot.
  * **_Untracked_** - Untracked files were not in the last snapshot and do not currently reside in the staging area.
### **The Life Cycle of File Status**
  * After you edit a file, Git flags it as modified because of changes made after the previous commit.
  * You stage the modified file.
  * Then, you commit staged changes.
# Remote Repositories
  * In order to collaborate on Git projects, you must interact with remote repositories, versions of a project residing online or on a network. You can work with multiple repositories, for which you can have read/write or read-only privileges. Teams can use remote repositories to push information to and pull data from.
## Cloned Repositories
  * As mentioned earlier, for cloned repositories, Git will automatically give the name “origin” to the server from which you cloned and the name “master” to your local branch.
## Seeing Your Remotes
  * By running the git remote command, you can view the short names, such as “origin,” of all specified remote handles.
  * By using git remote -v, you can view all the remote URLs next to their corresponding short names.


`$ cd example

$ git remote -v

remote1 https://github.com/remote1/example (fetch)

remote1 https://github.com/remote1/example (push)

remote2 https://github.com/remote2/example (fetch)

remote2 https://github.com/remote2/example (push)

remote3 https://github.com/remote3/example (fetch)

remote3 https://github.com/remote3/example (push)`
