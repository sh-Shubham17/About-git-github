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
> git add .  return
#Adds the files in the local repository and stages them for commit. To unstage a file, use  
git reset HEAD YOUR_FILE

- Commit the files that you’ve staged in your local repository.
> git commit -m 'First commit'
# Commits the tracked changes and prepares them to be pushed to a remote repository.
  To remove this commit and modify the file, use
git reset --soft HEAD~1
  And commit and add the file again.
