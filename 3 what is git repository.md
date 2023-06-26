# What is Git repository

Repositories in GIT contain a collection of files of various different versions of a Project. These files are imported from the repository into the local server of the user for further updations and modifications in the content of the file.<br>
Repositories can be divided into two types based on the usage on a server. These are:
- **Bare Repositories:** These repositories are used to share the changes that are done by different developers. A user is not allowed to modify this repository or create a new version for this repository based on the modifications done.
- **Non-bare Repositories:** Non-bare repositories are user-friendly and hence allow the user to create new modifications of files and also create new versions for the repositories. The cloning process by default creates a non-bare repository if any parameter is not specified during the clone operation.

# Working Tree or Staging of a git repository
A working tree in a Git Repository is the collection of files which are originated from a certain version of the repository. It helps in tracking the changes done by a specific user on one version of the repository.<br>
There are a few stages of a file in the working tree of a repository:
- **Untracked:** In this stage, the Git repository is unable to track the file, which means that the file is **never staged nor it is committed**.
- **Tracked:** When the Git repository tracks a file, which means the file is committed(already added to repo) but is not staged in the working directory.
- **Staged:** In this stage, the file is ready to be committed and is placed in the staging area waiting for the next commit.
- **Modified/Dirty:** When the changes are made to the file i.e. the file is modified but the change is not yet staged.

to Stage a file for next commit in working direcrory :
> git add <file-path>

and to discard changes in working directory if u have added file for commit:
> git restore <file>

After the changes are done in the working area, the user can either update these changes in the GIT repository or revert the changes.

# Adding to a Repository
GIT needs to follow two more steps to save these changes in the local repository. These steps are:
1. Adding the changes to the Index(Staging Area)
2. Committing the indexed changes into the repository

To add particular file only
> git add <file>

To add multiple files of a certain directory:
> git add .

To add changes in files across entire project
> git add --all

the main difference between the two commands is that "git add ." stages modifications and new untracked files in the current directory and its subdirectories but does not include file deletions. On the other hand, "git add --all" stages all changes, including modifications, new untracked files, and file deletions, across the entire project

To add all text files of the current directory to staging area.
> git add *.txt

To add all text files of a particular directory(docs) to staging area.
> git add docs/*.txt

To add text files of entire project to staging area
> git add “*.txt”

To commits the staged changes to the local repository.
> git commit -m "Add existing file"

This commit command is used to add any of the tracked files to staging area and commit them by providing a message to remember
<br>
<br>
