---
creation date: 2023-08-02 12:00
modification date: Wednesday 2nd August 2023 12:00:26
---

**Tags:** #DevOps #GIT 

### Source:
[Git](https://chat.openai.com/share/8fed5082-9761-42b4-b662-064f819b11c4)

--------------------------------------

### Overview of GIT:

##### 1. Repository(repo):
 * A repository is a storage location where all the versioned files and their history are stored.
 * It can be hosted remotely.
	 * GitHub
	 * GitLab
	 * BitBucket
* Or you can store locally

##### 2. Commits:
 * A commit represent a snapshot of the changes made to one or more files in the repository at a specific point  in time.
 * Each commit has a unique identifier(hash) and is associated with a commit message that describes the changes made.

##### 3. Branches:
 * Branches are used to work on new feature, bug fixes or experiments without affecting the main codebase
 * Default repo has a master/main branch.
 * Developers create a new branch and can merge them back into the main branch once the changes are tested and reviewed.

##### 4. Clone:
 * Cloning a repo means creating a local copy of the remote repo. this allows you to work on the code locally, make changes and then push those changes back to the remote repo.

##### 5. Pull/Push:
 * Pulling means fetching changes from the remote repo and merging them into your local branch.
 * Pushing means sending your local commits to the remote repo.

##### 6. Merge:
 * Merging combines changes from one branch into another.
 * When we merge branches, git tries to automatically reconcile the changes,
 * If there are conflicts, you will need to resolve them manually.

##### 7. Pull request:
 * Pull request is a request to merge changes from one branch into another.
 * If it's often used in collaborative projects, where contributors submit their changes for review before merging them into main branch.

##### 8. Staging area(index):
 * Before committing changes, Git allows us to stage specific changes for inclusion in the next commit.
 * This staging area helps you control which changes will be committed.


### Common `git` commands:

* `git init` -  Initializes a new GIT repo in the current directory
* `git clone <repo url>` - Clones a remote repo to local machine
* `git add <file` - Adds changes to the staging area.
* `git commit -m "Commit message"` - Create new commit with staged changes
* `git status` - Shows status of working directory and staging area
* `git branch` - Lists all branch
	* Asterix indicating current branch
* `git checkout <branch>` -  Switches to a different branch
* `git pull` - Fetches and merges changes from the remote repo to current branch.
* `git push` - Pushes local commits to remote repo
* `git merge <branch>` -  Merge the specified branch into current branch

#### Why it's important and what problem it solved among others:

* Widely used and essential tool in modern software development
* **Distributed Version Control:**
	* Which means, each developer has their own copy in local
		* This enables developers work offline, commit changes locally.
		* Collaborate effectively.
* **Efficient Branching and Merging:**
	* GIT branching and merging are powerful and lightweight
	* Creating and switching branch is very easy and fast
		* It will help developers to work in multiple feature or bugs simultaneously.
* **Data Integrity and Hashing:**
	* GIT uniquely identify each commit and data object in the repo.
	* it provide strong mechanism to detect corruption or tampering of data.
* **Rapid Operations and Performance:**
	* Mostly changes are performed locally
	* Only the changes are transferred over the network.

##### [[GIT real world experience]]


