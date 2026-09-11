henry is a boy

# Git Practice

A hands-on repository created to learn and practice Git and GitHub through practical exercises.

## Overview

This repository documents my practical learning of Git, focusing on how Git tracks changes, manages versions, and synchronizes a local repository with a remote GitHub repository.

The exercises were carried out using Git Bash and were designed to understand the Git workflow by working with actual files, folders, screenshots, and a Cisco Packet Tracer project file.

## What I Practiced

### 1. Initializing a Git Repository

Created a local project directory and initialized it as a Git repository using `git init`.

This created the `.git` directory, allowing Git to track changes and maintain the repository's history.

### 2. Tracking and Staging Files

Practiced adding files to the staging area using `git add`.

Files used during the exercises included:

* `README.md`
* Cisco Packet Tracer `.pkt` file
* Screenshots
* `.gitkeep` file for maintaining an otherwise empty directory

I also learned that Git tracks files rather than empty directories, which is why `.gitkeep` can be used as a placeholder when an empty folder needs to be included in a repository.

### 3. Creating Commits

Created multiple commits using `git commit -m` to save changes as checkpoints in the local repository.

This helped me understand that commits are stored in the local Git history and allow changes to be tracked over time.

### 4. Viewing and Comparing Changes

Used `git status` to check the state of the working directory and staging area.

I also practiced:

* `git diff` — viewing unstaged changes
* `git diff --staged` — viewing staged changes
* `git restore --staged` — removing changes from the staging area without deleting them
* `git restore` — discarding an unstaged change and returning the file to its last committed state

These exercises helped me understand the difference between the working directory, staging area, and committed history.

### 5. Viewing Commit History

Used `git log` and `git log --oneline` to inspect the repository's commit history and understand how Git records previous versions of the project.

### 6. Connecting the Local Repository to GitHub

Created an empty GitHub repository and connected it to the local repository using a remote named `origin`.

The remote was verified using:

`git remote -v`

This demonstrated that the local repository can be connected to a remote repository without immediately uploading its files.

### 7. Pushing the Local Repository to GitHub

Used:

`git push -u origin main`

to upload the local commits to the remote GitHub repository.

This was my first practical demonstration of how a local Git repository can be published to GitHub.

### 8. Synchronizing Local and Remote History

After the initial push, I modified the `README.md` file and created a new commit locally.

At this point, Git reported that the local `main` branch was **ahead of `origin/main` by one commit**. This demonstrated that the new commit existed locally but had not yet been pushed to GitHub.

I then used:

`git push`

to send the new commit to the remote repository.

GitHub's `main` branch was updated, bringing the local and remote histories back into synchronization.

## Git Workflow Practiced

The main workflow practiced in this repository was:

```text
Modify files
    ↓
git status
    ↓
git diff
    ↓
git add
    ↓
git diff --staged
    ↓
git commit
    ↓
git status
    ↓
git push
    ↓
Remote GitHub repository synchronized
```

## Key Lessons

Through this hands-on practice, I learned that:

* Git is a version control system used to track changes and manage project history.
* GitHub provides a remote platform for hosting Git repositories.
* `git add` stages changes for a commit.
* `git commit` saves a checkpoint in the local repository.
* `git push` transfers local commits to the remote repository.
* `git status` helps identify whether changes are unstaged, staged, committed, ahead of the remote, or synchronized.
* Local and remote repositories can have different histories until changes are pushed or pulled.
* Git allows changes to be reviewed before they are committed.

## Purpose

This repository serves as a practical foundation for using Git and GitHub in future networking, Linux, cloud, and cybersecurity projects.

