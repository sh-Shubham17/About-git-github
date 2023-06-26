# What GIT is about?

Git is a free and open-source distributed version control system designed to handle everything from small to very large projects with speed and efficiency


# Why Use Version Control Software?

Version control software allows the user to have “versions” of a project, which show the changes that were made to the code over time, and allows the user to backtrack if necessary and undo those changes.


# Characteristics of Git

1. Strong support for non-linear development
2. Distributed development
3. Compatibility with existing systems/protocol
4. Efficient handling of large projects
5. Data Assurance
6. Automatic Garbage Collection.
  1. Git automatically performs garbage collection when enough loose objects have been created in the repository.
  2. Garbage collection can be called explicitly using
  > git gc –prune.


# How does GIT work ?

1. A Git repository is a key-value object store where all objects are indexed by their SHA-1 hash value.
2. All commits, files, tags, and filesystem tree nodes are different types of objects living in this repository.
3. A Git **repository is a large hash table with no provision made for hash collisions**.
4. Git specifically works by taking **“snapshots”** of files
