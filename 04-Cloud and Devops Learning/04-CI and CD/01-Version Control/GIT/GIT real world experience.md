---
creation date: 2023-08-02 16:32
modification date: Wednesday 2nd August 2023 16:32:54
---

**Tags:** #DevOps #GIT 

#### Source:
[Git](https://chat.openai.com/share/8fed5082-9761-42b4-b662-064f819b11c4)

--------------------------------------

### Overview about practice:

#### Steps to do:

1. **Choose an open source project**
	 1. Project with well documented
	 2. Clear contribution guide
2. **Fork repo:**
	1. Forking creates a copy of the project under our Github account.
	2. We can freely modify it
3. **Clone the forked repo:**
	1. Clone your forked repo to our local machine
		1. By using `git clone`
4. **Study the project structure:**
	1. Understand about directory structure
	2. Understanding source code
	3. Directory layout
	4. Configuration files
5. **Create a new Branch:**
	1. Before making any changes, create a new branch
		1. `git checkout -b <branch-name>`
	2. By creating branch we can isolate a changes from the development branch.
6. **Start Making changes:**
	1. Now we do changes
		1. Fix bugs
		2. Add new feature
		3. Improve documentation
7. **Commit the changes**
	1. use `git add` to stage the changes
	2. `git commit -m "commit message"`  to create a commit with a descriptive message about the changes you made
8. **Pull the latest changes:**
	1. Regularly pull latest changes from original repo to local branch to keep fork up to date
	2. use `git pull upstream <branch>` 
		1. `upstream` --> Original repo
		2. `<branch>` --> Branch want to sync
9. **Push changes and create pull requests:**
	1. Once changes are made push branch to our forked repo
		1. Using `git push origin <branch>`
	2. Then create a pull request from our branch to the original repo
	3. The pull request will allow project maintainers to review changes and potentially merge them into the main codebase
10. **Code review:**
	1. Code reviews are an essential part of the open-source development process and will help you improve your skills.

### Usefule Resources:

1. https://codeberg.org/explore/repos
2. 
#### [[1. Git Practice -First Contribution]]
