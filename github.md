# What is GitHub about?

Github is an online platform where we can share our codes(or projects) online hassle-free. Github is place where we host our local git repository online. it basically allow you to work collaboratively within a group of peoples. It hosts all the features of Git and have its own too.

Github is owned by Microsoft, provides access to public(free) and private(paid) repositories. It allows free repository to host files up to 100mb and total size for 2GB.


# How to upload existing repository to GitHub

- The system should have **git installed** in it if not install git. Make sure to choose Run git from Windows Command prompt option during installation. Otherwise, open git bash in place of step 2.
- Change the current working directory to your local project.
- Initialize the local directory as a git repository in different ways as described in the image.
> git init

- A **new .git folder** is created in the directory which is by **default hidden**.
- Add the files in your new local repository. This stages them for the first commit.
> git add . <br>
Adds the files in the local repository and stages them for commit. To unstage a file, use <br>
git reset HEAD YOUR_FILE

- Commit the files that you’ve staged in your local repository.
> git commit -m 'First commit'<br>
// Commits the tracked changes and prepares them to be pushed to a remote repository.


To remove this commit and modify the file, use
> git reset --soft HEAD~1  

And commit and add the file again


To set a main branch at local repository:
>  git branch -M main


to set remote to repo where u want to host ur code:
> git remote add origin URL


to push ur changes in ur local repo to GitHub:
>  git push -u origin main


### Note :
1. **git push origin main:**
This command pushes the commits from your local branch named "main" to the remote repository named "origin". However, without the "-u" option, it does not establish an upstream tracking relationship between your local branch and the remote branch. As a result, you will need to specify the remote branch explicitly in future push commands, like "git push origin main" each time you want to push to that branch.

2. **git push -u origin main:**
This command also pushes your local "main" branch's commits to the "origin" remote repository. However, the "-u" option has an additional effect. It establishes an *upstream tracking relationship* between your local branch and the remote branch. It means that Git remembers the association between your local "main" branch and the "origin/main" branch. After using this command, you can simply use **"git push"** without any additional arguments in the future. Git will know that you want to push to the "origin/main" branch by default

You may download changes from remote repository to local repository using the command:
>git pull
